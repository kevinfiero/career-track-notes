* Architectual Style and Patterns [Link](https://medium.com/@mlbors/architectural-styles-and-architectural-patterns-c240f7df88a0#:~:text=Architectural%20Patterns%20VS%20Design%20Patterns&text=In%20a%20few%20words%2C%20while,and%20mechanisms%20of%20a%20system.)
  * Architectual patterns are high level whereas design patterns impact specific sections of code.
  * Patterns:
    * Layered - divides architecture into logic parts such as the presentation, application, business logic, and data access layers.
    * Event-Driven -consists of emitters and consumers.
    * Domain Driven Design - organizes according to the domain or business use cases.
    * Pipes and Filters - scrubbing and transporting data can be separated.
    * Microservices - creating several tiny programs instead of one monolith.
* Container and Presentation Pattern [Link](https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/)
  * Containers (state and logic) are separted from the presentation layer (what is rendered to the user).
* Container Details [Link](https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/container-details)
  * Containers handles tasks mostly related to state such as initializing data, setting state, and fetching data.
* Presentation Details [Link](https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/presentation-details)
  * Presentation handles the displayed of elements on the page.
* Functional vs. Class Components [Link](https://medium.com/@Zwenza/functional-vs-class-components-in-react-231e3fbd7108)
  * Advantageous to write a functional component on a presentation layer without state.
  * When using a functional component the advantages include:
    * Easier to read and test
    * Less code
    * Easier to conform to best practices
    * Performance boost
* Conditional Rendering [Link](https://reactjs.org/docs/conditional-rendering.html)
  * Components can be rendered conditional similar to how logic operators are used in normal JavaScript.
