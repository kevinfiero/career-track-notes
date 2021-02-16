* Redux Motivation [Link](https://redux.js.org/introduction/motivation)
  * Redux was created to help manage state.
  * Helps mutate state and deal with asynchronicity
* Redux Three Principles [Link](https://redux.js.org/introduction/three-principles)
  * Repeat of yesterday's reading
* Redux Core Concepts [Link](https://redux.js.org/introduction/core-concepts)
  * Repeat of yesterday's reading
* Redux Actions [Link](https://redux.js.org/basics/actions)
  * One-way data flow: state --> actions --> view --> state --> ...
  * Redux allows a single centralized place to maintain global state.
  * To update objects immutably a copy must be made before the change occurs.
  * Actions contain a type (descriptive name for the action) and payload (additional information about what happened).
  * Reducers have rules to follow:
    * Calculate new state based on state and action arguments.
    * Changes must be done immutably.
    * Asynchronous logic or side-effects can not occur.
  * To update the store the dispatch must be called.
* Redux Reducers [Link](https://redux.js.org/basics/reducers)
  * Tutorial to walk through a basic React application using Redux.
