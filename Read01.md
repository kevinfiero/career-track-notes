* Destructuring - [Link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
    * Array Destructuring
        * Destructuring allows a variable to be accessed in an array using distinct variables.
        * Use the rest keyword to return the remaining values in an array:
            ```
            let a, b, rest;
            [a, b, ...rest] = [10, 20, 30, 40, 50];
            console.log(rest) // [30, 40, 50]
            ```
        * Assigning default values if the array unpacked results in an undefined variable:
            ```
            let a, b;
            [a=5, b=7] = [1];
            console.log(a); // 1
            console.log(b); // 7
            ```
        * Can swap variables in single destructuring assignment:
            ```
            let a = 1;
            let b = 3;
            [a, b] = [b, a];
            console.log(a); // 3
            console.log(b); // 1
            ```
        * Destructuring variables returned from a function:
            ```
            function f() {
                return [1, 2];
            }

            let a, b; 
            [a, b] = f(); 
            console.log(a); // 1
            console.log(b); // 2
            ```
        * You can also ignore values returned from a function by omitting them in the return:
            ```
            function f() {
            return [1, 2, 3];
            }

            const [a, , b] = f();
            console.log(a); // 1
            console.log(b); // 3

            const [c] = f();
            console.log(c); // 1
            ```
        * Ignore all returned values:
            ```
            [,,] = f();
            ```
        * Assign the rest of the array to a variable:
            ```
            const [a, ...b] = [1, 2, 3];
            console.log(a); // 1
            console.log(b); // [2, 3]
            ```
        * You can unpack values from a regular expression match as well.
    * Object Destructuring
        * Similar to array destructuring:
            ```
            const user = {
                id: 42,
                is_verified: true
            };

            const {id, is_verified} = user;

            console.log(id); // 42
            console.log(is_verified); // true 
            ```
        * Can assign to new variable names:
            ```
            const o = {p: 42, q: true};
            const {p: foo, q: bar} = o;
 
            console.log(foo); // 42 
            console.log(bar); // true
            ```
        * Can assign default values:
            ```
            const {a = 10, b = 5} = {a: 3};

            console.log(a); // 3
            console.log(b); // 5
            ```
        * Can unpack object literals for function calls:
            ```
            const user = {
                id: 42,
                displayName: 'jdoe',
                fullName: {
                    firstName: 'John',
                    lastName: 'Doe'
                }
            };

            function userId({id}) {
                return id;
            }

            function whois({displayName, fullName: {firstName: name}}) {
                return `${displayName} is ${name}`;
            }

            console.log(userId(user)); // 42
            console.log(whois(user));  // "jdoe is John"
            ```
        * Can use destructuring in nested objects and for-of iterations.

* Rest - [Link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters)
    * Rest parameters can be used at the end of a user supplied input to assign remaining values to a single array. This is true even if there is only one value or no value in the array.
    * Can use a map function to multiple the first value in the array by other values and return that result:
        ```
        function multiply(multiplier, ...theArgs) {
        return theArgs.map(element => {
            return multiplier * element
        })
        }

        let arr = multiply(2, 15, 25, 42)
        console.log(arr)  // [30, 50, 84]
        ```
    * Rest array is a real array whereas the arguments object is not.

* Spread - [Link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)
    * Spread syntax looks the same as rest syntax but functionally does the opposite. Rest syntax condenses multiple elements into a single element, whereas rest syntax expands an array into its elements.
    * Example:
        ```
        function myFunction(v, w, x, y, z) { }
        let args = [0, 1];
        myFunction(-1, ...args, 2, ...[3]);
        ```
    * The spread syntax can be used multiple times and does not need to be the last argument, as seen above.
    * The spread argument eliminates the need for code bloat to accomplish the same task of array manipulation by use of push(), splice(), or concat().
    * Spread syntax only goes one level deep which makes it unsuitable for multi-dimensional arrays.
