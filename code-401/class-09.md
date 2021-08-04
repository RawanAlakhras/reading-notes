# WRRC and Java

# The HTTP Request Lifecycle

## Local Processing

* Your browser extracts the "scheme"/protocol (we have established
that this will be HTTP), host (www.example.com),
and optional port number, resource path, and query strings that are specified in the form
* Now that the browser has the intended hostname for the request, it needs to resolve an IP address1. The browser will then look through its own cache of recently requested URLs, the operating system’s cache of recent queries, your router’s cache, and your DNS cache.

## Resolve an IP

*  resolving an IP from a "DNS server"2 is a sequence that includes many steps, and includes failovers if the first request fails to return an address.
* If the cache lookup fails (we will assume it does), your browser fires off a DNS request using UDP3. 
* The DNS request contains the preconfigured IP for your DNS server and your return IP in its header. 
*  The hostname for which you are trying to resolve an IP is in the request’s "Question" section. UDP is a lightweight protocol, but the tradeoff is that it offers no guarantees in terms of delivery, and there is no acknowledgement other than a response being sent and received.
* Your request will now have to travel many network devices to reach its target DNS server. 
* Whenever the packet hits a piece of networking equipment, the device uses a routing table to determine which other device it is connected to that is most likely situated along the shortest path to the destination.4
* Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname. If it finds one, it sends a response. If, on the other hand, the DNS server you have targeted cannot locate the given hostname, it passes the request along to another DNS server it is configured to defer to. 
* We will assume the request is successful though, given that all of this is still a precursor. If the response makes it back (remember, with UDP there’s no guarantee!), the requesting client now has a target IP. It will also have received a piece of information as part of the answer that will let it know how long the returned answer can be cached for. 

## Establish a TCP Connection

* One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission.
* These guarantees and more can be found on Wikipedia, and are worth reading about, but what’s most relevant is that TCP connections are opened using what’s known as a three-way handshake.
* The client initiates the active open by sending a SYN7 "control"8 packet to the server.
* The server responds with a SYN-ACK9 message, which contains an acknowledgement number for the original message that is always x+1, and a new sequence number for the response itself, which is another random number y.
* In the third step, the client sends an ACK10 message back to the server with a sequence number equal to x+1, which should match the SYN-ACK message’s acknowledgment number and ensure that our data is being delivered reliably. The ACK message’s acknowledgment number (since it is acknowledging the SYN-ACK) is set to one more than the received sequence number, or y+1.

## Send an HTTP Request

* The request is made up of a "request line", request header, and a body.
* Once the HTTP request is sent, it follows a similar routing procedure as the one discussed earlier, with the difference being that using TCPs magic sequence number powers, the server can ensure it receives the whole request, in the correct order.
* Once the server receives the request, processes it, and finds the resource being requested, it generates an HTTP response. 
* Once the response is generated, the server responds to the request. At the TCP layer, the client receives the first data packet, the first byte of which should contain the HTTP response header. 


## Tearing Down and Cleaning Up

* Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.
* At this point, your browser begins processing what it has received. If it is an image, data, or other media file that is being consumed by some application inside the browser, a variety of things can happen.
