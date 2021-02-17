* Understanding Redux [Link](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/)
  * Really enjoying this explanation of Redux. Going to continue reading this over the next few days.
* Redux Hooks [Link](https://react-redux.js.org/next/api/hooks)
  * Hooks are currently going over my head at the moment. I think I need to get more of the fundamentals down.
* Redux Fundamentals [Link](https://redux.js.org/tutorials/fundamentals/part-2-concepts-data-flow)
  * One-way data flow: state --> actions --> view --> state --> ...
  * Redux allows a single centralized place to maintain global state.
  * To update objects immutably a copy must be made before the change occurs.
  * Actions contain a type (descriptive name for the action) and payload (additional information about what happened).
  * Reducers have rules to follow:
    * Calculate new state based on state and action arguments.
    * Changes must be done immutably.
    * Asynchronous logic or side-effects can not occur.
  * To update the store the dispatch must be called.
