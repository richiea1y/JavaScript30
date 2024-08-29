# JavaScript30 Day 2 - CSS + JS Clock

## Introduction

![alt text](image-1.png)

### Main goals

- Making this pretty sweet CSS clock
- It takes in the current time from JavaScript, and it’s going to update these hands, second, hands based on the current hour, minute, second.

### Demo: [Click me](https://richiea1y.github.io/JavaScript30/Day2-CSS+JS-Clock/)

## ✏️ Notes

### 1. Creating a right-side pivot point for rotation using the CSS transform-origin property

- Origin [(`transform-origin` (MDN))](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin) is where it’s going to do the rotation off of. So transform-origin: 100%; that will do along the x-axis (By default, it’s 50%).

- It changes where it goes off of and a 100% along the x-axis will put that pivot point on the very right-hand side.

### 2. Position the clock hands to start at 12 o'clock by adjusting the CSS transition property

- Because divs are block and they’re left to right, it’s not actually starting at 12:00.

- We could just rotate the entire thing by default, 90 degrees. `transform: rotate(90deg)`;
  We can say `transition: all 0.05s;`. Now it’ll tick itself around.

### 3. Using transition-timing-function for an ease-in-out effect

- `transition-timing-function: ease-in-out;` It eases itself in and out.

- Then also going to take `transition` down to `0.05s` seconds, just nice and quick.

### 4. To execute a function in JavaScript every second, you can use the setInterval() method.

- This will execute the function every seconds (1000 milliseconds).

  ```JavaScript
  function setDate() {
    console.log('Hi');
  }

  setInterval(setDate, 1000);
  ```
