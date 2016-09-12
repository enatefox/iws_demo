Helpdesk Ticketing System Demo

This is a demonstration of a ticketing system utilizing the following technologies (subject to change):

-- Flask web server
-- MySQL
---- SQLAlchemy to follow but not currently implemented
-- Python for Flask itself
-- HTML, CSS and JS
-- Currently using jQuery for development speed but to be moved to Knockout.js when apt to do so (the actual demo is working)

Implementation requires a very bare-bones Python run from CLI or scripted as one may be wont to do. 

Quick breakdown of architecture (as this is public, for general consumption by readers, please do not simply try to pull and run out-of-the-box):
-- Backing store database is holding `users` and `tickets` as noted in the source. 
-- User reaches site and either registers or logs in.
-- If the email (their ID) isn't in the system, they are registered and can view their tickets or others as defined by role (this is not written at this point in time).
-- The existing tickets will be displayed in a single-pane view and the options to update or create new ones are then offered (I'll try to work on making it shiny and move around all pretty with blurred backgrounds and sliding forms, etc. depending on time).
-- Option to respond to tickets with comments, reply to users- both submitters as well as clients to follow.
---- This will most likely not be completed for this but allow for this demo, the user to get to the form to see the conceptual idea of it.
