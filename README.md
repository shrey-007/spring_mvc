A simple Spring MVC project which where Dispatcher Servlet(Front Controller) handles all the requests and delegate it to respective servlets.
pom.xml=dependencies of project
web.xml=it maps servlets to different url pattern
spring-servlet.xml=for creation of beans like viewResolver
Explaination-:
Whenever a new url is entered then it first go to front controller(Dispatcher Servlet) and then it identifies which controller should recieve the request.
supoose you fire /home so first request will go to front controller and then it will identify which controller has @RequesMapping("/home").It is same as in servlet and jsp program finds which servlet matches the url pattern. so it finds that home() method will handle the /home request so it runs the home() method and then home()
returns the "home" string to frontcontroller which gives this string to viewResolver whose bean you have to create yourself, it identifies the whole path of the view and give it back to frontcontrooler and then front controller diaplays home.jsp

It only has one controller which will fire when you append /home to url.
local repo project=mvc_new
