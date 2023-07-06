# apetalk

A tree-walking interpreter for the Monkey language.

## Code examples

```javascript
let num = 10 * (20 / 2);

let add = fn (a, b) { 
    return a + b;
};

add(5, num); // => 105

// recursion
let fibonacci = fn(x) {
    if (x == 0) {
        return 0;
    }

    if (x == 1) {
        return 1;
    }

    fibonacci(x - 1) + fibonacci(x - 2);
};

// higher order functions
let twice = fn(f, x) {
    return f(f(x));
};

let addTwo = fn(x) {
    return x + 2;
};

twice(addTwo, 2); // => 6
```

