#### Ember

Ember provides the client-side framework plus development tooling, conventions and standards.
Ember packages up all the build tools and best-practices.

- To install ember npm install -g ember-cli
-g is to install the package globally, making package executables available everywhere on the system.


#### Routers in Ember
The router manages your app state and maps it to the path to the URL
Router keeps track of what an application user is doing and where someone is at in your application at all times.
Routes are configured under app/router.js - Router.map function.

#### Links in Ember
To avoid full page refresh and hardcoding HTML link; Use the Handlebars {{link-to}} expression to navigate while avoiding page reload.