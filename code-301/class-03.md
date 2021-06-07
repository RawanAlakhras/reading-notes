# Passing Functions as Props

* map() return an Array 
* we can loop through an array and display each value in JSX using react in this way 

```javascript
    const numbers = [1, 2, 3, 4, 5];
    const doubled = numbers.map((number) => number * 2);
    console.log(doubled);

```

* Each list item needs a unique key .
* Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

# Spread Operator

* JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

## List 4 things that the spread operator can do:
1. The spread syntax “spreads” the array into separate arguments.
2. Copying an array
3. Concatenating or combining arrays
4. Using Math functions


