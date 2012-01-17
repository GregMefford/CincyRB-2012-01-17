Warbler
=======

Lots of companies are heavily invested in hosting J2EE apps and often have
"a guy" or "a gal" who knows all about it.

A common way to deploy Java web applications is with a single *WAR (Web
application ARchive) file*. It's just a *fancy ZIP file with particular
structure and metadata files*.

Warbler offers the following for JRuby users:

* Turns Rails/Sinatra/Camping/Rack/Whatever app into a WAR file
* The WAR file can be put in a standard Java Servlet container (like Tomcat)
* Everything just works by magic with minimal pain

To use:
-------

    jruby -S gem install warbler
    mkdir config && warble config # Creates config/warble.rb

Edit config/warble, or grab an example from https://github.com/jruby/jruby-rack/blob/master/examples/

    warble

Then, plop the .war file in Tomcat's @webapps/@ directory and it should work
like magic!

(Disclaimer: Tomcat can be fussy and it won't actually always work)
    
