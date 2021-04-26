# Local Storge

* local storage is one of the areas where native client applications have held an advantage over web applications.
* the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.
* These values may be stored in the registry, INI files, XML files, or some other place according to platform convention.
* Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data.
* Cookies have three potentially dealbreaking downsides:
    1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
    2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
    3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

* Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.
* userData allows web pages to store up to 64 KB of data per domain .
* IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.
* In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects.
* Briefly, it allows Flash objects to store up to 100 KB of data per domain. Brad
  
### INTRODUCING HTML5 STORAGE

* What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.

* what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. 
* you’ll access HTML5 Storage through the localStorage object on the global window object. 

### USING HTML5 STORAGE

* HTML5 Storage is based on named key/value pairs.
* You store data based on a named key, then you can retrieve that data with the same key. 
* The named key is a string. The data can be any type supported by JavaScript
* the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

```javaScript
interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};

```
