"Enterprise" Ruby
=================

Or: "How do use Ruby in an environment heavily entrenched in Windows and Java."

JRuby
-----

JRuby is an implementation of the Ruby interpreter written in Java. That means
that it runs normal Ruby code, but the program actually doing the reading and
executing is written in Java.

![JRuby Download Links](pictures/JRuby_downloads.png)

* Takes advantage of tons of effort that went into making the JVM fast
* Works well on Windows
* Access to Java's libraries
* Threading works well
* Takes forever to start, but runs well once it's going

![JRuby Start Menu](pictures/JRuby_start_menu.png)

Warbler
-------

Lots of companies are heavily invested in hosting J2EE apps and often have
"a guy" or "a gal" who knows all about it.

A common way to deploy Java web applications is with a single *WAR (Web
application ARchive) file*. It's just a *fancy ZIP file with particular
structure and metadata files*.

Warbler offers the following for JRuby users:

* Turns Rails/Sinatra/Camping/Rack/Whatever app into a WAR file
* The WAR file can be put in a standard Java Servlet container (like Tomcat)
* Everything just works by magic with minimal pain

Bonus: Trinidad
---------------

Blissful JRuby web application server.

* Uses Tomcat under the covers
* Absurdly easy to install and use

OCRA (One-Click Ruby Application)
---------------------------------

Windows users like to have something to double-click. OCRA turns a Ruby script
into a Windows .EXE file that they can easily click to run without installing
Ruby or any other special dependencies.

* Very simple to use
* Magically figures out what gems need to be baked into the EXE
* You can tell it other resource files to bake in, too
* Compresses itself to save space (by default)
* Takes forever to start up, but runs well once it's going