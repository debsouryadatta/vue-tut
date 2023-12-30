# vue-todos

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```


### Steps of learning:
1. npm init vue@latest
2. choosing router - yes, Baki sab - no
3. cd vue-todos, npm i, npm run dev
4. Using <script setup> in the script tag, its a syntactic sugar to avoid the need to import vue and define the component inside the setup function.(Normally all the variables and functions are defined inside the setup function)

5. Overview of vue project - defineProps(just like react), slot in vue - to pass template content to the child component
6. Deleting all the stuff and starting from scratch, npm i --save-dev uid sass @iconify/vue, importing google fonts(Rubik)
7. Putting some basic styles in the App.vue style tag
8. Creating the TodoHeader component and adding it to the App.vue
9. The scope in the styled tag makes sure that the styles are applied only this component
10. Changing the HomeView component to TodosView component
11. Creating TodoCreator component inside TodosView component, const todo = ref("") -> ref is a reactive function, it makes sure that the value is reactive(changing the value will cause the component to re-render)
12. Another way of taking inputs -> Using todoState(reactive functions)
13. Implementing emit function to pass the todoState to the parent component, listening the emit on the parent component and creating the todo in the todoList

14. Changing the todo to todoState, changing the createTodo func accordingly, understaning the difference between v-if & v-show directives, adding dynamic classes using `:class` directive
15. Understanding how slot works, using slot in the button component
16. Creating TodoItem component, using v-for="todo in todoList" directive to loop through the todoList
17. Showing all the todos and displaying the icons & input box conditionally in the TodoItem component
18, In vue, we can't change the value of props directly in the child component, we need to emit the event and change the value in the parent component
19. Passing index as a prop to the TodoItem component, using the index to update the todo, defining an emit when the input checkbox changes
20. Updating(completing, editing, changing value, deleting) the todoList in the TodoView component using the emit from the TodoItem component

21. Creating setTodoListLocalStorage & fetchTodoList functions to store and fetch the todoList from the localStorage
22. Using watch function from vue to watch the changes in the todoList and updating the localStorage accordingly(Using the deep property to be true for better watch)
23. Using computed function from vue to get the completedTodos and remainingTodos, and showing the message accordingly
24. Understanding the lazy loading in the router, using the lazy loading in the routes
25. Deploying the site.