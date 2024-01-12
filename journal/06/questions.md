# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > The entrypoint of an application is where the execution of the program starts, it is the 'main' method

02. What is the difference between a vue `component` and `page`?

  > Components are a feature that makes up part of the user interface, it is used for parts of your application that you will potentially re-use in multiple places. examples are modals, forms, display cards. A page is a part of an application that can be navigated to & takes in everything that is needed to build the user interface that the user will interact with. For example, home page, about page, products page.

03. What is ***Component-Based Architecture***?

  > Component based architecture incorporates components into the application. So instead of writing out the code to display a feature, it get encapsulated into a component file & is then referenced into where it will display on a page.

04. What are the three tags that make up a Vue component?

  > the 3 tags are: Template, where you utilize HTML. Script, where you utilize Javascript. & Style, where you utilize CSS/SCSS

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > Lifecycle hooks are special methods that allow you to execute code at specific points in the lifecycle of a vue component. They are used to execute code before/during creation, before/during mount, before/during update & before/during destruction.

06. Which component in Vue does the vue-router use to mount pages onto?

  > The router-view is where components mount onto the page. It is a placeholder where the matching component will be rendered.

07. What is the difference between the `AppState` and the state object within a component?

  > The AppState is the 'single source of truth', it is where data is stored & drawn from & there is only one in an application. the state object in a component is data that is specific to that component.

08. What is the responsibility of `Services` in our Vue projects?

  > The responsibilities of the services in our Vue projects is the same as in the MVC projects. It holds all of our 'business logic'. It holds most of out executable functions which we reference into our .vue pages (which acts as a combination of our view & controllers when we did MVC)

09. What are ***props*** and how are they used? Provide an example

  > Props allow us to move data from our page to our component. If you have a modal component & need to input data to a form & update the AppState/api with that user data then you need to use props to access & transfer that data. That allows components to be more versatile so one component can be reused effectively in different places.

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > Vue has reactive features like ref, computed & onMounted that allow us to watch objects & update as they are changed. The method that we use specifically to create a watchable object in the AppState is computed.
