# Flexbox-CssGrid

Created by Vince Chang </br>

Experimenting with the different layouts of flexbox and css grid.

### Cupcakes

- Description: This app was built to .
- Useful links:
  ![Flexbox-grid](http://flexboxgrid.com/)
  ![Flexbox-froggy](https://flexboxfroggy.com/)
  ![Flexbox-defense](http://www.flexboxdefense.com/)

### Questions:

    1. Ask a question here
       - answer

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

### Flexbox

- Parent (flex container) and child (flex item)
- Good for centering
- Easy to reorder boxes
- **Disadvantage**: Works only in 1-D
- Flex container is like a wrapper
- Flex items live inside the Flex container
- Flex-basis = "width" like a relative number, never use the width property on flex items, always use flex-basis because width is an absolute number, flex basis is more flexible

### Flexbox as a grid
