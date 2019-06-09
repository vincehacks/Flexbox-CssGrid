# Flexbox-CssGrid

Created by Vince Chang </br>

Experimenting with the different layouts

### Projects

### Netflix

- Description: This app was built to reflect what Netflix would look like. Tech
  Stack was React, ES6, CSS5, along with Jest testing.
- Functionality:
  - Users can search for a show and see only hits for that search
  - Can click on a show card and view details about that show
    ![Landing](https://github.com/vincehacks/ReactJS/blob/master/netflix/FinalProduct1.png)
    ![Shows](https://github.com/vincehacks/ReactJS/blob/master/netflix/FinalProduct2.png)
    ![Search](https://github.com/vincehacks/ReactJS/blob/master/netflix/FinalProduct3.png)

### Questions:

    1. When should I use `extends Component`? Instead of extend React.Component
       - They are ideally the same, but {Component} will just import the
       Component itself and not the whole Library itself. Rule of thumb, is
       import only the things you need.

    2. Where do you need to call ReactDOM.render() ? Every file or just in the
       main?
       - Just in the main, the <App> container

    3. Is className suppose to be a CSS class that you create yourself?
       - className is reserved

    4. When you render multiple components you need to have keys
       - This will avoid the warning, for React's rendering, it needs to know if it can reuse the component

    5. Show example of import and export components, do you separate components
       by file? Or is it better to have more than one component in the same
       file?
       - Depends on what you are trying to build

    6. Why do we pass in props in a constructor and why do we have to call
       super?
       - Only use constructor if it has a state and if you want to attach a
       function to it, we call super to initialize the the component. Javascript prototype

    7. What does this.bind do and if you didn’t use it, what would 'this' refer
       to?
       - If I didn’t bind it, it would refer to the actual function that I'm
       calling it in as oppose to the component itself

    8. Why do I have to export 'App'?
       - I have to import app to index.js (this is the entry point). create-
       react-app will give index.js to index.html as a minified version!

    9. What does export default COMPONENT do?
       - Tells exactly which component to use. If there were two+ components,
       it would be confusing as to which component to use/import

    10. !== compares both type and value and != just compares value

### Defining Responsive Design

- 3 Characteristics of Responsive Design:
  1. Media Queries
     - browser reports the screen resolution
     - based on the width, utilize the appropriate stylesheet
     - no javascript involved
  2. Images that resize
     - images should change size based on screen resolution
     - can have client side or server side solutions
  3. Grid base layout
     - consist of columns and rows

### Floats

- Was used in the past for layout of webpages as a hack after table layouts
- features rows and cells
- rows are responsible for clearing the cells
- source order determines the display
- **Major Disadvantage** is that floats have equal column heights
