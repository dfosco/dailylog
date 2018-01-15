# JS30 Notes

These are notes on Wes Bos' [JavaScript30 course](https://javascript30.com/)

---

### Day 1
#### JS Drum Key

 - Add event listener to any key pressed on the window

```javascript

window.addEventListener('keydown', function (e) {
  console.log(msg)
});

```

### Day 2
#### JS and CSS Clock

```css
transform-origin: 100%;
/* Translates the origin point for transformation along the X axis */
```

### Day 3
#### Update CSS Variables with JS

 - Data attributes add items to the object of the DOM node they're at. Cool!

 ```javascript
  const suffix = this.dataset
 ```

### Day 4
#### Array Cardio Day 1
 - Filter: takes an array and filters it to less items than the original

 - Map: Takes an array and gives back a new array -- like a factory machine, that takes a raw material and transforms it, without loss (takes 10 items, return 10 different items)

 - Sort: It... well, sorts the items. It does that by adding a value to an array item if it matches the criteria, and subtracting if it doesn't. Sort goes through all of the items in the array and when it's done, they are sorted with index values in order.

 - Reduce: Loops over the array items accumulating value according to what's specified in the function to reduce it to a single value

---

**About Callback Functions (aka high-order functions)**

In JavaScript, functions are first-class objects; that is, functions are of the type Object and they can be used in a first-class manner like any other object (String, Array, Number, etc.) since they are in fact objects themselves. They can be “stored in variables, passed as arguments to functions, created within functions, and returned from functions”1.


http://javascriptissexy.com/understand-javascript-callback-functions-and-use-them/

---

**JUMP TO DAY 11**

---

### Day 11
#### Hold Shift to Check Multiple Checkboxes

 - A good way to capture click events:

```js
const checkboxes = document.querySelectorAll('element-selector')
function handleCheck(e) { console.log(e) }
checkboxes.forEach(checkbox => checkbox.addEventListener('click', handleCheck))
```
