# Spring Security Architecture

## Authentication and Access Control

* The security of an application can be divided into two main portions:
    1. Authentication : To determine if a user is authenticated.
    2. Authorization : What an authenticated user is allowed to do Sometimes people say “access control” instead of "authorization".

## Authentication

* The main strategy interface for authentication is AuthenticationManager .
* An AuthenticationManager can do one of 3 things in its authenticate() method:
    1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.
    2. Throw an AuthenticationException if it believes that the input represents an invalid principal.
    3. Return null if it cannot decide.
* AuthenticationException is a runtime exception. It is usually handled by an application in a generic way, depending on the style or purpose of the application.
* The most commonly used implementation of AuthenticationManager is ProviderManager, which delegates to a chain of AuthenticationProvider instances.
* An AuthenticationProvider is a bit like an AuthenticationManager, but it has an extra method to allow the caller to query whether it supports a given Authentication type

## Authorization or Access Control

* After authentication is done successfully authorization can be done after that.
* The main strategy used in the framework is AccessDecisionManager.
* ConfigAttribute is the interface used to handle authorization methods.
* Has one method that have the accessed roles.

## Web Security

* Spring web security is based on servlet filters.
* The proccess can be illustrated in chaining a number of ordered filters that is applied to a request until it reaches a client or server.
* FiltersChainProxy is the first filter implemented with spring security.
* The security filters are @Bean's in the ApplicationContext.
* FilterChainProxy is the parent of all implemented filters.
* By extending configure method from WebSecurityConfigurerAdapeter and the class that holds it can be annotated with the Order annotation to give a priority to each secured class.
* Request matchers are configurations used to apply security to a specific HTTP requests.
* Securing a method is that the user have to go through security authentications to execute the method useing the secured annotations.

# Spring Auth Cheat Sheet

* Step 1: set up a user model and repo
* Step 2: create a controller for that model
* Step 3: UserDetailsServiceImpl implements UserDetailsService
  * gets a User from the database by username (make sure your repository has the method to make this easy!)

* Step 4: ApplicationUser implements UserDetails
  * use IntelliJ to implement the methods; make the boolean ones all return true

* Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
  * has a UserDetailsService
  * passwordEncoder bean
  * configure AuthManagerBuilder
  * auth.userDetailsService(userDetailsService).passwordEncoder(passwordEncoder());
  * configure HttpSecurity
  * cors? csrf?
  * matchers for URLs that are allowed
  * ensure that login and signup URLs allowed; also consider homepage etc.
  * formLogin with login page set up
  * logout

    ``` java
    @Override
    @Bean
    public AuthenticationManager authenticationManagerBean() throws Exception {
        return super.authenticationManagerBean();
    }
    ```

* Step 6: registration page
  * create it w/ form
  * ensure it posts to a route your controller is ready for
  * check it's saving in the DB

    ```java
    // maybe autologin?
    Authentication authentication = new UsernamePasswordAuthenticationToken(newUser, null, new ArrayList<>());
    SecurityContextHolder.getContext().setAuthentication(authentication);
    ```

* Step 7: login page
  * create it w/ form
  * ensure it posts to the route you specified in web config
  * try it out!
  * add to a template w/ things about the Principal
