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

- {{link-to}} generates an anchor tag.
- The generated anchor tag can be customized by passing additional parameters to {{link-to}} tag. For eg: class="orders-link"
- Most Handlebars helpers accept a tagName property to change the generated HTML. As shown below if tagName is div, Ember will generate a div tag. And even though it will be generated as div, ember still knows to watch for clicks on it and it will still perform navigations.
{{#link-to "orders" class="orders-link" tagName="div"}}orders{{/link-to}}

#### Additional Ember Helpers
|debugger   |Stop processing to enter the debugger       |
|each       |Iterate over a collection of objects        |
|if         |Conditionally render the section of contents|
|input      |Create an HTML input element                |
|link-to    |Create an HTML anchor element               |
|log        |console log from simple debugging           |
|textarea   |Create an HTML textarea element             |
|unless     |Conditionally render the section of contents|

#### Routes in Ember
Ember CLIprovides a generator for creating a route and updating a router.
- To generate a route we can use:
- ember generate route <route-name>

Routes are defined in app/routes with a filename matching their route name.
- To customize the route's model - The Model Hook returns the data used in the route and its template.
- Using Model here is an Ember convention. Model represents the primary piece of data that the route represents and makes available to its templates.

#### Service in Ember
Service are long-living objects (aka, "singletons") that areavailable throughout your app.
- To generate a service we can use:
- ember generate route <service-name>
