* MVC [Link](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)
  * Model - Central component that manages the data, logic, and rules of the application.
  * View - Components that represent information.
  * Controller - Accepts inputs and converts it to commands for the model or view.
* Architecture of Single Page Applications [Link](https://hackernoon.com/architecting-single-page-applications-b842ea633c2e)
  * Domain Layer
    * Domain
      * Represents the state
    * Domain Services
      * Encapsulates business logic
      * Side-effect free
  * Store Layer
    * Store
      * Holds the state
      * State is immutable
      * Acts as a publisher
      * Notifies subscribers about state changes
  * Application Services
    * Project (interpret) state
    * orchestrate external operations
  * View Layer
    * Presentational Components
      * Receive state through props
      * Emit new state through events
    * Container Components
      * Receive state from the store
      * Supply state to presentational components
      * Send new state to the store
* React MVC [Link](https://blog.testdouble.com/posts/2019-11-04-react-mvc/)
  * An example of using MVC patterns in React.
* Reconciliation [Link](https://reactjs.org/docs/reconciliation.html)
  * React uses diffs to partially render only what has changed therefore preventing everything needing to be reloaded every time a change occurs.


