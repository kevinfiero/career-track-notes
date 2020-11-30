* Quantity Trumps Quality - [Link](https://blog.codinghorror.com/quantity-always-trumps-quality/)
    * This short article drives home the point that software engineers should learn by having hands on keyboard and figuring things out through trial and error. By sitting and thinking about the perfect solution it is often less beneficial than trying it out and tweaking it.

* Clean Code: Chapter 1 - [Link](http://ptgmedia.pearsoncmg.com/images/9780132350884/samplepages/9780132350884.pdf)
    * Code will need to be written by humans for the foreseeable future as creativity and vague requirements will make it difficult to be automated.
    * Bad code written will eventually become unmanageable and too hard to modify or maintain. Rushing can lead to short-term wins but ultimately may put a company out of business in the long run.
    * The prime culprit of bad code is rushing through it for one reason or another and vowing to clean it up later. However, this seldom happens as there is always more to get done.
    * Increasing productivity and pressure by management leads to a boiling point of developers demanding to slow down or management hiring more staff with little returns.
    * It is important to stand up to managers who do not understand the design of the code. Timelines need to slow down or something has got to give so that the development process can output clean code.
    * Programmers need "code-sense" to know what clean and bad code looks like and how to write clean code.
    * Reduce dependencies, making the code easy to read, optimizing speed, naming conventions, memory leaks, etc. are all principles of making the code clean.
    * Bad code tries to do too much in a single module.
    * According to Ron Jeffries avoiding duplication and repetitive logic is a good aspect to strive toward as it eliminates other issues. Another factor is to be expressive with variables, methods, etc. so the code is readable.
    * There are many schools of thought about writing clean code. None of these are objectively right or wrong but developers prescribe to one or another as a sort of guiding star.
    * Boy Scout Rule - make things cleaner than when you found it. This could be changing a small line of code and does not need to be a massive refactoring overhaul.

* TDD Red-Green-Refactor - [Link](https://www.codecademy.com/articles/tdd-red-green-refactor)
    * Three phases:
        * Red — think about what you want to develop
            * Since this is the first phase and no code is written, it is assumed the test will fail.
        * Green — think about how to make your tests pass
            * Implement the code to get the failing test to work but do not go beyond this.
        * Refactor — think about how to improve your existing implementation
            * Once the test works make the code easy to read, faster, or some other benefit while still getting the test to pass.

* Cycles of TDD - [Link](https://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html)
    * Three laws of TDD:
        * Create a unit tests that fails
        * Write production code that makes that test pass.
        * Clean up the mess you just made.
    * Refactoring should be done in a cycle along the course of the project lifetime rather than at the end.
    * Tests will be very specific at first but the code becomes more generic as time goes on. This requires the developer to revisit the prior tests and delete, add, or refactor so that more edge cases are accounted for in the tests.
    * Developer should be certain to evaluate their code and test structures at an hourly interval to ensure the bigger picture is not getting lost in the weeds.