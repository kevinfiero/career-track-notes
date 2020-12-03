* Promise - [Link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
    * Promises are an alternate use of async / await. They allow a proxy for a value that is not yet known. Commonly, when reaching out to an API, the promise will eventually expect something to be returned. In the mean time it is in a pending status until it is ultimately fulfilled or rejected.
    * Promises can be chained with .then and .catch methods. This allows further actions to be taken on the initial promise or catch an error that occurs.

* Video - [Link](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
    * JS call stack behaves as a last-in-first-out (LIFO) algorithm.
    * Recursive function will continue to add to the call stack until Chrome terminates it.
    * The stack blocks the browser from executing more code which is why callbacks are necessary.
    * Event Loop will place an item from the task queue onto the stack if the stack is empty. 
    * setTimeout of 0 and 5000 in the trivial example will arrive back to the stack after everything is executed. So these may effectively be doing the same thing if the stack takes awhile to clear.
    * Render queue has priority over the callback queue. Neither can be executed while the call stack has items in it.