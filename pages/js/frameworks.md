---
title: Frameworks
permalink: /javascript/frameworks/
layout: docs
sidenav: js
---
# Frameworks

**We recommend using [React]() for projects when possible.** As a team, we enjoy using React because it has a strong component model, enables easy server side rendering, and faciliates debugging by making the UI elements a function of the application state. React is most akin to the "view layer" in an MVC (Model-View-Controller) architecture and is frequently used with some other libraries. In our projects, we tend to use:

* [Redux](https://www.npmjs.com/package/redux) for managing state
* [Webpack](https://www.npmjs.com/package/webpack) and [Babel](https://babeljs.io/) for compiling our Javascript

However, we are not dogmatic about React - we just vastly prefer it. Here are some other popular frameworks that have been used at 18F and some of their key characteristics.

## Angular
AngularJS (commonly referred to as "Angular") is an open-source web application framework maintained by Google and by a community of individual developers and corporations to address many of the challenges encountered in developing single-page applications ([Wikipedia](http://en.wikipedia.org/wiki/AngularJS)).

#### When to use:
- Sites with heavy front end, JavaScript UI interactions (single page apps) such as:
  - creating, updating, deleting of information without a server reload
  - real-time messaging platforms, such as chat or complex messaging such as email
  - complex data visualization dashboards
  - lazy-loaded from the back end
- When the site's design specifies a single page app architecture over classic server request and response.
- When the whole site will be built with Angular to maintain front end code consistency.

#### When not to use:
- For a single or a few simple components (with the rest of the site not using Angular), instead see React or Web Components.
- Exporting a module that isn't an Angular module.
- If there is a strict requirement that the site should work for users that have JavaScript disabled.
- If there already is an active M**V framework (Backbone, ampersand, Ember) being used on the site.
- When the site's design doesn't benefit from a single page app architecture.
- When the long-term maintenance dev team is very unfamiliar with Angular and don't have the resources to learn or hire for it.

#### Pros:
- Takes care of a lot of boilerplate code for front end interactions.
- Attempts to extend HTML itself, and was designed so less experienced devs could use it.
- Being maintained and developed by Google generally means good support.

#### Cons:
- While open source, is maintained primarily by Google.
- Has been known to implement breaking changes in major version updates.
- Built with Typescript and Dart, both of which are not ECMA standardized (as opposed to vanilla JS or ES6).
- Has a steep learning curve and is very opinionated, meaning you learn Angular rather than JavaScript.


## Backbone
Backbone.js is a JavaScript library with a RESTful JSON interface and is based on the model–view–presenter (MVP) application design paradigm ([Wikipedia](http://en.wikipedia.org/wiki/Backbone.js)).

#### When to use:
- A page design that requires dynamic data manipulation on the front end without a server request response, such as a todo app.
- When a small front end framework is required due to performance constraints.
- When the long-term dev maintenance team is unfamiliar with any full frameworks, such as Angular.
- To use as a wrapper and rest data manipulation library around a view-only framework, such as React.
- When the dev team is familiar enough with Backbone to know how to write maintainable Backbone code.

#### When not to use:
- When the JavaScript components don't keep data or manipulate data, in which case Backbone's functionality is too heavy and not specific enough for just view rendering.
- If there is a strict requirement that the site should work for users that have JavaScript disabled.
- When another full JavaScript framework is already in use, such as Angular.
- When working with a data source that is NOT RESTful. Backbone was built for RESTful services, instead see Flux.

#### Pros:
- Relatively un-opinionated, meaning a lot of freedom in development.
- Open source, and has an active, large community.

#### Cons:
- Still requires a lot of boilerplate code (this can be mitigated by pairing with a library like Marionette)
- Since it has very little structure, inexperienced programmers can easily create unmaintainable code with Backbone.
- Designed primarily for REST data.


