* Array Methods - [Link](https://dev.to/frugencefidel/10-javascript-array-methods-you-should-know-4lk3)
    * 10 JavaScript Array Methods:
        1. forEach() - loop over an array similar to a for loop
        1. includes() - returns a boolean on whether the array contains the specified value
        1. filter() - creates a new array with only elements matching the criteria
        1. map() - applies function to every element in array
        1. reduce() - returns a single accumulated value based on the contents of the array
        1. some() - returns a boolean of whether at least one element meets the criteria
        1. every() - returns a boolean if all elements meets the criteria
        1. sort() - arranges the array in either ascending or descending order
        1. Array.from() - creates array-like elements into an array
        1. Array.of() - creates an array of the elements passed into it
* Array Method Cheat Sheet - [Link](https://jrsinclair.com/javascript-array-methods-cheat-sheet)
    * This contains two diagrams that give summaries of array functions. 
* TDD, Where Did It All Go Wrong - [Link](https://www.youtube.com/watch?v=EZ05e7EMOLM)
    * Stay at a company long enough and you'll stumble on your own mistakes.
    * A lot of people leave before they run into their own issues and it causes future developers to bear the burden of bad code.
    * Should be able to run tests that are not specific to certain data sets or scenarios. This makes it so tests break when code is refactor.
    * Some have the philosophy that TDD slows developers down and a few bugs in production and getting feedback is more beneficial.
    Customers don't engage with test suites but a lot of time goes into maintenance.
    * TDD by Example by Kent Beck is where the ideas started. A lot of people learn about TDD from others and haven't actually read the pitfalls and those solutions.
    * Write a new test if a new functionality (or behavior) is introduced. This is often a high-level user requirement. Avoid testing implementation details.
    * If a behavior changes then a test should change to capture the new behavior.
    * During the 'green' step get the test by any means possible even if that means copying and pasting elsewhere. But also important to go back and refactor. When you refactor you change the implementation details but not the result.
* TDD Red-Green-Refactor - [Link](https://www.codecademy.com/articles/tdd-red-green-refactor)
    * Three phases:
        * Red — think about what you want to develop
            * Since this is the first phase and no code is written, it is assumed the test will fail.
        * Green — think about how to make your tests pass
            * Implement the code to get the failing test to work but do not go beyond this.
        * Refactor — think about how to improve your existing implementation
            * Once the test works make the code easy to read, faster, or some other benefit while still getting the test to pass.
* Cycle of TDD - [Link](https://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html)
    * Three laws of TDD:
        * Create a unit tests that fails
        * Write production code that makes that test pass.
        * Clean up the mess you just made.
    * Refactoring should be done in a cycle along the course of the project lifetime rather than at the end.
    * Tests will be very specific at first but the code becomes more generic as time goes on. This requires the developer to revisit the prior tests and delete, add, or refactor so that more edge cases are accounted for in the tests.
    * Developer should be certain to evaluate their code and test structures at an hourly interval to ensure the bigger picture is not getting lost in the weeds.