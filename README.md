# Cosemo
Server Module Framework for Containers

## Background
When coding for the web there are some questions always emerging when you want to create the backend
* Which programming language and framework should be used?
* How to do login?
* Where should I host the backend?
* Is it possible to get a HA setup cheap, and easy to code?
* Which database should be used?
* How can I scale my file system?
* How do I do backups?
* How many users can I serve easily in the future if the service grow?
* Which security measures should I use?
* Can I have persistent sockets?
* How do I test my code?

## Containers
Containers are emerging as a paradigm to how to host backend applications. There is a lot of work
put into orchestration of them, and a lot of companies try to switch their old monolithic
applications into micro-services. But as a developer or Ops guy I still have many questions which
I need answers to.
* Which orchestrator should I use?
* How should I write my interface between services?
* Can I reuse services created by others in my setup?
* What about security between containers?
* Where is the documentation for the services?
* Can I have a system to test external services?
* Loadbalancing build into the orchestrator or create my own?

## What if
What if we could have a framework where all these questions didn't need answers? A framework where
I can write my code in almost any language I want, document the API in the requests, plugin
any service I want from others, only write my code and skip all the bloated lines of code
just to manage all?

This is the reason Cosemo was created. It is a framework which tries to minimize the code a backend
developer need to write to be able to handle all the stuff you always need to handle.

## Framework
So what will Cosemo handle?
* Command based modules with json payload and gRPC as internal transport
* Managing module
* Log module
* A router module which will be frontend into the system. This will be scalable
* A interconnect which will connect all the services with each other and the routers
* Security between all services through the managing module and interconnects
* Swappable user module for handling user info and login
* Streaming endpoints which you can redirect streaming services to
* All connection code for services
* Defining all aspect of a service as json a object

And a lot more.

## Example

