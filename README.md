# jsflogin
jsflogin
1.	Overview of your application and a brief description of the system architecture and interconnection among the tiers.

Below is a brief description of how I envisaged the archecture would look.
Application was modelled on a three tier MVC architecture (Model ,View ,Controller). (The XHTML files provide the view which is the user interface. This is built from JSF components , these allow a visual GUI to be built that can be populated from and interface to a backend database , theses Faclet components populate JSF managed beans and these interface with the controllers that provides the business logic tier. These controllers contain EJB (enterprise java beans and its these that talk to the JPA ( Java persistence architecture) entities that are persisted to the backend database via an entity manager.
The Welcome screen has links to the Register user, Book flight, and List itinerary screens
All screens have links back to the Welcome screen.


2.	How to run your application.

Choose inde.html click run on server. The application is not complete so will only allow registration of user, flights, 

3.	Design of the components with reasons of why a particular (bean) technology is used in the application.

Login bean –  session bean set on initial entry to sight records if user login in or not status of which opens up screens like print ticket , view itinerary.

Flight bean – request bean pulls information about flight from database for display once in display can be discarded.

Booking Bean – session bean user can move between screens allows data to be written back to database on each move with status falg non committed so allow partial saving of data..

