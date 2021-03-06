Vertx experiment - Real time Dropwizard dashboard
=======================================

This was just a weekend experiment to refresh my Javascript knowledge and try out some technologies I've been looking at for some time.
Don't expect it to be of production quality or that I'll maintain it.

Dropwizard is a well instrumented and productive framework for building production ready restful web services. It exports a lot of statistics on a admin port. I thought it would be fun to create a proxy polling this endpoint and feeding the data to clients connected via web sockets. The proxy is implemented using the fairly new Vertx framework enabling highly concurrent polygot application development on the JVM.

While I was working on the client side of the dashboard I thought it would be fun to have a look at Knockout.js for data binding. I quite liked the declarative way it solves a lot of common problems related to data binding.

Latest update
---------------
Started upgrading Vertx and Bootstrap to their latest versions.


Screenshots
------------
![CSS dark](https://github.com/edeoliveira/dropwizard-dashboard/raw/master/screenshots/dashboard.png)


Give it a spin
--------------

Fire up a Dropwizard project with the admin interface running on port 8081.

When Dropwizard is running it should only be a matter of running `./gradlew run` and point your browser to http://localhost:9000/.

_Ps! This will download and install Gradle in your home folder!_


Relevant technologies and libraries
-------------------------------------
http://vertx.io/

http://dropwizard.codahale.com/

http://knockoutjs.com/

http://momentjs.com/

http://smoothiecharts.org/

https://developers.google.com/chart/



Things to do
-------------

**Ditch Knockout:** It does not bring much to the table for this application. Just accidental complexity.

**Introduce tabs:** The dashboard is too long. Perhaps it would be a good idea to introduce tabs + a small page with a quick overview.


Contributions
--------------

Big thanks to [Daniel Mayo](https://github.com/dmayo3) for his contributions! This was just an evening project and I'd never thought that anyone would pick it up.

-------------------
[![endorse](http://api.coderwall.com/kimble/endorsecount.png)](http://coderwall.com/kimble)