A simple Spring MVC project which where Dispatcher Servlet(Front Controller) handles all the requests and delegate it to respective servlets.
pom.xml=dependencies of project
web.xml=it maps servlets to different url pattern
spring-servlet.xml=for creation of beans like viewResolver
It only has one controller which will fire when you append /home to url.
local repo project=mvc_new
