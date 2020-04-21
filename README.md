Pallavi Darisi

Student NO-190678627

email id: p.darisi


Implementing RESTful services in Python and Flask

Building web services with Flask is surprisingly simple, much simpler than building complete server side applications.

There are a couple of Flask extensions that help with building RESTful services with Flask, but the task is so simple that in my opinion there is no need to use an extension.

The one of our web service will be asking the service to add, remove and modify tasks, so clearly we need to have a way to store tasks. The obvious way to do that is to build a small database, but because databases are not the topic of this article we are going to take a much simpler approach.

In the place of a database we will store our task list in a memory structure. This will only work when the web server that runs our application is single process and single threaded. This is okay for Flask's own development web server. It is not okay to use this technique on a production web server, for that a proper database setup must be used.
