# Flex Box and CSS Grid

Created by Vince Chang </br>

Experimenting with the different layouts of flex box and css grid.

#### USEFUL LINKS

[Flex Box-grid](http://flexboxgrid.com/) </br>
[Flex Box-froggy](https://flexboxfroggy.com/) </br>
[Flex Box-defense](http://www.flexboxdefense.com/) </br>

#### DEFINING RESPONSIVE DESIGN

- 3 Characteristics of Responsive Design:
  1. **Media Queries**
     - browser reports the screen resolution
     - based on the width, utilize the appropriate stylesheet
     - no javascript involved
  2. **Images that resize**
     - images should change size based on screen resolution
     - can have client side or server side solutions
  3. **Grid base layout**
     - consist of columns and rows

#### FLOATS

- Was used in the past for layout of webpages as a hack after table layouts
- features rows and cells
- rows are responsible for clearing the cells
- source order determines the display
- **Major Disadvantage** is that floats have equal column heights

#### RESPONSIVE IMAGES

- Images that should change size based on screen resolution
- Load times might be long
- Can solve with server-side

#### FLEX BOX

- Parent (flex container) and child (flex item)
- Good for centering
- Easy to reorder boxes
- **Disadvantage**: Works only in 1-D
- Flex container is like a wrapper
- Flex items live inside the Flex container, only the direct children of the
  flex container are considered flex items!
- Flex-basis = "width" like a relative number, never use the width property on
  flex items, always use flex-basis because width is an absolute number, flex
  basis is more flexible

#### FLEX-DIRECTION

```css
row
row-reverse
column
column-reverse
```

#### FLEX-CONTAINER

- Area of document laid out using Flex Box

```css
display: flex
display: inline-flex

This will turn all children into flex items
```

#### FLEX-WRAP

- Wrap onto multiple lines

```css
flex-wrap: wrap;
```

#### FLEX-FLOW (Flex direction + Flex wrap)

```css
flex-flow: direction wrap

Where direction is either: row OR column
Where wrap is is either: wrap OR nowrap
```

#### FLEX ITEM PROPERTIES

1. **flex-basis**
   - Defines the size of an item in terms of space it leaves as available space
   - Initial value is `auto`
   - Looks to see if items have a size
   - What is the size of the item before growing and shrinking happens?
2. **flex-grow**
   - Set to a positive number
   - Specifies the flex-grow factor and determines how much the flex item will
     grow relative to the rest of the flex items in the flex container when the
     positive free space is distributed
   - How much of the **positive** free space does this item get?
3. **flex-shrink**
   - Can shrink only if total values overflow the main axis
   - flex-grow adds space and flex-shrink takes away space
   - If there is not enough space in the container to layout items and
     flex-shrink is set to a positive -int, the item can become smaller than the
     flex-basis
   - How much **negative** free space can be removed from this item

**Flex Shorthand**

```css
flex: flex-grow, flex-shrink, flex-basis;
```

#### PROPERTIES THAT CONTROL ALIGNMENT

Main axis = the one I define
Cross axis = the opposite of main axis

1. **align-items**
   - Align items on the **cross axis**
   - Initial value is **stretch**, which is why flex items stretch to the
     height of the tallest one by default
2. **justify-content**
   - Align items on the **main axis**
   - Initial is **flex-start**
   ```css
   space-between = equal space around
   space-around = equal space right and left
   space-evenly
   center
   flex-start
   flex-end
   ```
3. **align-self**
   - Align items of an individual item
4. **align-content**
   - Controls space between flex lines on the cross axis

#### THE ORDER PROPERTY

- Target individual items and change where they appear in the visual order with
  the order property
- Default order is: 0
- Can give negative values if you want to make one item display first and leave
  the rest of the order alone

#### FLEX BOX VS CSS GRID

- Flex Box = 1D Layout
- Grid = 2D layout
- Flex items can wrap, but once that happens, each line becomes a flex container
  but in Grid you can control row and column
- Possible to use both Grid and Flex Box together
- Rule of thumb: If adding widths to flex items in order to make items in one
  row of a wrapped flex container line up with items above them, then use Grid for
  2D layout
- Use Flex Box for **small** components and Grid for **larger** ones, but not
  always the case!
