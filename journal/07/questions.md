# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > One way binding is interpolating with mustache brackets {{ }}
  two way data binding uses v-model which allows data to move both ways, so it can take in information from a model & then input user data

2. The `SPA` acronym stands for what?

  > It stands for single page application

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > faster loading times, fewer server requests, encourages modular development, just to name a few

4. What does the `onMounted` method in Vue do?

  > on mounted runs on page load

5. What is the `v-model` attribute in Vue for, and when might you use it?

  > It is used for two way data binding which allow it to take in user data & create a new object based on a model. We have used it to take in form data to create new posts

6. What is the package.json file used for?

  > It is for Node.js & npm & serves several purposes related to project configuration, dependencies & metadata

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > v-if, v-else, v-else-if, v-show

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > it is used when rendering lists of elements, it helps vue identify items & makes DOM updates more efficient 

9. What is the `<slot>` element and what is it used for?

  > it is used for reusable & customizable components. Mick used it on Gregslist to make a very flexible modal that could be used different ways by different parts of the application.
