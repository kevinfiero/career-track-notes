* setState Explained [Link](https://css-tricks.com/understanding-react-setstate/)
  * setState allows the component to update the relevant part of the DOM. This is why React is fast.
  * Using setState allows the page to render again. Do not update state directly.
  * Calling setState multiple times will not work as only the last call wins out. TO avoid this pass a function instead.
  * It is important to use an updater when accessing previous state.
* Lists and Keys [Link](https://reactjs.org/docs/lists-and-keys.html)
  * Can be collections of elements using lists with JSX.
  * React elements need to have unique keys so what changed can be identified.
  * Keys only need to be unique amongst an element's siblings.
* Typechecking Props [Link](https://reactjs.org/docs/typechecking-with-proptypes.html)
  * propTypes allows data to be validated.
  * propTypes can allow default values. 
* Components and Props [Link](https://reactjs.org/docs/components-and-props.html)
  * Review of React Components and Props.
* Handling events [Link](https://reactjs.org/docs/handling-events.html)
  * Review of handling events in React.
* Snapshot Testing [Link](https://jestjs.io/docs/en/snapshot-testing)
  * Tests the UI for changes against a snapshot.
* React Testing Library [Link](https://kentcdodds.com/blog/introducing-the-react-testing-library)
  * React testing library focuses on the way the user will interact with the software rather than implementation details.
