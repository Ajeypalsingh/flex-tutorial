## FLex Property

The ```flex property``` is used in CSS (Cascading Style Sheets) to control how flexible
an element should be within a flex container. Flexbox is a powerful layout mechanism 
that allows you to create ```dynamic``` and ```responsive layouts``` with relative ease.
By using the flex property, you can define how much space an element should take up within the flex
container, as well as how it should ```grow``` or ```shrink``` in relation to other elements

### Creating a Flex Container

To create a ```flex container```, you’ll first need to select an element to be the container. This could be any HTML element, such as a ```div``` or ```section```.

```HTML
   <div class="container">
       <section>
          <div class="box box-1"></div>
          <div class="box box-2"></div>
          <div class="box box-3"></div>
          <div class="box box-4"></div>
       </section>
    </div>
```

```CSS
section {
    display: flex;
}
```
Once you apply the display: flex; property to the container, the elements inside will automatically become flex items.

### Controlling Flex Items

There are several properties you can use to control the behavior of the flex items within a flex container.
```flex-direction```

The flex-direction property determines the direction in which the flex items are laid out within the container.
```By default```, this is set to row, which means the items will be laid out ```horizontally```. You can also set it to
column to lay out the items vertically.

### flex-grow and Flex Shrink

The ```flex-grow and Shrink``` property controls how much an item should grow or Shrink to fill any available space within 
the container. By default, all items have a value of 0, which means they won’t grow  at all. If you set a value greater 
than 0, the item will grow proportionally to the amount of available space.

```CSS
.box {
    flex-grow: 0;
    flex-shrink: 1;
    flex-basis: 160px;
}
```
