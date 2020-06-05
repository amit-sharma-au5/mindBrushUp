# Interiew Questions

### Name the DIfferent Life cycle methods?
[Life cycle](https://programmingwithmosh.com/javascript/react-lifecycle-methods/#:~:text=React%20component%20lifecycle%20has%20three,It%20is%20a%20pure%20function "React Life cycle")

---

### What are the controlled components?
`functional components are uncontrolled component and class components are controlled. Because we can control input in class componenet using state change. where we manage componenet from state basically`

--- 

### How do you tell React to build in Production mode and what will that do?
` npm run build`

---

###  What is a higher order component?
`A higher order component is function that a takes a componenet and returns a new component. A higher-order component (HOC) is an advanced technique in React for reusing component logic. HOCs are not part of the React API, per se. They are a pattern that emerges from React’s compositional nature.`

--- 

### advantage using arrow function
` arrow functions are less verbose than traditional functions arrow functions take the this from their surronding`

### Why is it advised to pass a callback function to setState as opposed to an object?
 Because this.props and this.state may be updated asynchronously, you should not rely on their values for calculating the next state. 
 Normally the problem not occur, but if we have multiple datas then this problem might occur that's why we should use function to set state

[Function vs Object](https://medium.com/@wisecobbler/using-a-function-in-setstate-instead-of-an-object-1f5cfd6e55d1#:~:text=Function%20in%20%60setState%60%20to%20the%20rescue!&text=Passing%20in%20a%20function%20into,your%20component's%20state%20and%20props%20.)

---

### What is the alternative of binding `this` in the constructor?

--- 

### How would you prevent a component from rendering?
pure Component vs should Component Update
[Link](https://www.robinwieruch.de/react-prevent-rerender-component#:~:text=React's%20shouldComponentUpdate%20Method&text=As%20you%20can%20see%2C%20the%20shouldComponentUpdate%20class%20method%20has%20access,%2C%20the%20component%20re%2Drenders.)

---
     
### What does "shouldComponentUpdate" do and why is it important?
Use shouldComponentUpdate() to let React know if a component’s output is not affected by the current change in state or props. The default behavior is to re-render on every state change, and in the vast majority of cases you should rely on the default behavior.
This method only exists as a performance optimization. Do not rely on it to “prevent” a rendering, as this can lead to bugs. Consider using the built-in PureComponent instead of writing shouldComponentUpdate() by hand. PureComponent performs a shallow comparison of props and state, and reduces the chance that you’ll skip a necessary update.
[Link](https://reactjs.org/docs/react-component.html#shouldcomponentupdate)

---
     
### What is JSX?
[Link](https://reactjs.org/docs/introducing-jsx.html)

---
     
### What is equivalent of the following using React.createElement?
  JSX is not a requirement for using React. Using React without JSX is especially convenient when you don’t want to set up compilation in your build environment.
  [Link](https://reactjs.org/docs/react-without-jsx.html)

---

### What is a store in redux?
A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it.

A store is not a class. It's just an object with a few methods on it. To create it, pass your root reducing function to createStore.
[Link](https://redux.js.org/api/store)
     
### What is an action?
An action is a plain object that represents an intention to change the state. Actions are the only way to get data into the store. Any data, whether from UI events, network callbacks, or other sources such as WebSockets needs to eventually be dispatched as actions.

Actions are payloads of information that send data from your application to your store. They are the only source of information for the store. You send them to the store using store.dispatch().
[Link](https://redux.js.org/glossary#state)
[Link](https://redux.js.org/basics/actions#:~:text=Actions%20are%20payloads%20of%20information,to%20the%20store%20using%20store.)

--- 

### What don't you like about React?
  1. It's just a library, not a framework like Angular.

  2. When the application loads initially, there is no cache of JavaScript in the browser. If the application is    big, the time taken to initially load the application will also be huge.
  3. Since the application is rendered in the client side, the web crawlers that search engines use won’t be able to index the JavaScript generated content. The search engines will see your application to be blank and then rank you poorly.

---

### What can you tell me about JSX?
    JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.
---
     
### Name some popular Flux Libraries
     
### What are stateless components?
stateful components are keeping track of changing data, while stateless components print out what is given to them via props, or they always render the same thing.
[Link](https://programmingwithmosh.com/javascript/stateful-stateless-components-react/)
     
---
      
### What is the difference between createElement and cloneElement?
createElement is what JSX gets Transpiling to create React Elements (object representations of some UI).
cloneElement is used in order to clone an element and assign it new props

---

### What's the difference between a "smart" component and a "dumb" component?
Same as state componenet or stateless Componenet.

---
     
### What is the render method for?
The render() method is the only required method in a class component.
The render() function should be pure, meaning that it does not modify component state, it returns the same result each time it’s invoked, and it does not directly interact with the browser.

---
     
### What are some limitations of things you shouldn't do in the component's render method?
You cannot modify the component's state (with setState), nor interact with the browser (do that in componentDidMount). Render should be a pure function.

---
     
### What's an alternative way to avoid having to bind to this in event callback methods?

     
### What is the point of using keys in React?
It allows for more efficient rendering of lists, so that React can reuse DOM elements without having to destroy + recreate them when lists change (slightly) in the UI.
[Link](https://github.com/WebPredict/react-interview-questions)

---
     
### What's the typical pattern for rendering a list of components from an array of data?
Call map on an array with an arrow function that executes for each array element, possibly outputting a React component for each.
[Link](https://github.com/WebPredict/react-interview-questions)

---
     
### What is reconciliation in React?
It's React's process of re-rendering its tree of UI components.
[Link](https://github.com/WebPredict/react-interview-questions)

---
     
### What's the difference between an Element and a Component in React?
Elements are the fundamental building blocks of React, and describe what you want to see on the screen. They are just simple JS objects with props, key, ref, and type properties, whereas Components have a render method and optionally accept inputs.
[Link](https://github.com/WebPredict/react-interview-questions)

---
  
### What is the point of shouldComponentUpdate() method?
    It's used for performance reasons, for example if the implementor of a component knows for sure that a particular property change does not necessitate a re-render, they could return false from this method and skip the re-render.
[Link](https://github.com/WebPredict/react-interview-questions)

### What are PropTypes in React?
They help indicate to React what data types a React component's properties are and should accept.
[Link](https://github.com/WebPredict/react-interview-questions)

### What is ReactDOM?
It's a top-level React API to render a React element into the DOM, via the ReactDOM.render method.

---
     
### What are typical middleware choices for handling asynchronous calls in Redux?
  1. Redux Thunk, 
  2. Redux Promise, 
  3. Redux Saga

---

### What's the typical flow of data like in a React + Redux app?
Callback from UI component dispatches an action with a payload, which then is intercepted in a reducer, possibly producing a new application state, which is then propagated down through the tree of components in the application from the Redux store.

---

### What are Pure Components?
PureComponent is exactly the same as Component except that it handles the shouldComponentUpdate method for you. When props or state changes, PureComponent will do a shallow comparison on both props and state. Component, on the other hand, won’t compare current props and state to next out of the box. Thus, the component will re-render by default whenever shouldComponentUpdate is called.
[Link](https://github.com/sudheerj/reactjs-interview-questions)

---

### Why should not we update the state directly?
If you try to update state directly then it won’t re-render the component.
Instead use setState() method. It schedules an update to a component’s state object. When state changes, the component responds by re-rendering
[Link](https://github.com/sudheerj/reactjs-interview-questions)
     
---

### What is the difference between HTML and React event handling?
[Link](https://github.com/sudheerj/reactjs-interview-questions#what-is-the-difference-between-html-and-react-event-handling)

---
     
### How to bind methods or event handlers in JSX callbacks?
[Link](https://github.com/sudheerj/reactjs-interview-questions#how-to-bind-methods-or-event-handlers-in-jsx-callbacks)

     
### What are synthetic events in ReactJS?
SyntheticEvent is a cross-browser wrapper around the browser's native event. It's API is same as the browser's native event, including stopPropagation() and preventDefault(), except the events work identically across all browsers.

---

     
### What is Key and benefit of using it in lists?
     
### What are forward refs?
[Link](https://github.com/sudheerj/reactjs-interview-questions#what-are-forward-refs)
     
### What is the difference between ShadowDOM and VirtualDOM?
The Shadow DOM is a browser technology designed primarily for scoping variables and CSS in web components. The virtual DOM is a concept implemented by libraries in JavaScript on top of browser APIs.
[Link](https://github.com/sudheerj/reactjs-interview-questions#what-is-the-difference-between-shadow-dom-and-virtual-dom)
     
### What are uncontrolled components?
The Uncontrolled Component are the one that stores its own state internally, and you query the DOM using a ref to find its current value when you need it. This is a bit more like traditional HTML
For example, in the below UserProfile component, the name input accessed using ref as below,
[Link](https://github.com/sudheerj/reactjs-interview-questions#what-are-uncontrolled-components)

---

### What is the difference between createElement and cloneElement?
JSX elements will be transpiled to createElement JS syntax to create React elements which are going to be used for the object representation of UI. Whereas cloneElement is used to clone an element and pass it to new props.
[Link](https://github.com/sudheerj/reactjs-interview-questions#what-is-the-difference-between-createelement-and-cloneelement)
     
### What is Lifting State Up in ReactJS?
     
### What are the different phases of ReactJS component lifecycle?
     
### What are the lifecycle methods of ReactJS?
     
### What is children prop?
     
### How to set state with a dynamic key name?
     
### What would be the common mistake of function being called every time the component renders?
     
### Why ReactJS uses className over class attribute?
     
### Why fragments are better than container divs?
     
### What are error boundaries in ReactJS (16)?
     
### What are the advantages of React over VueJS?
     
### What do these three dots (...) in React do?
     
### What are advantages of using React Hooks?
     
### What are React Hooks?
     
### What's the difference between `useRef` and `createRef`?
     
### What is useState() in React?
     
### What is StrictMode in React?
     
### Why do class methods need to be bound to a class instance?
     
### What is prop drilling and how can you avoid it?
     
### What is the purpose of super(props)?
     
### What is "Children"?
     
### Why would you eject from create-react-app?
     
### What is a reducer?
     
### Are you familiar with Flux?
     
### Describe Flux vs MVC?
     
### If you created a React element like Twitter below, what would the component definition of Twitter look like?
      
### What is the difference between a controlled component and an uncontrolled component?
     
### Why would you use React.Children.map(props.children, () => ) instead of props.children.map(() => )?
     
### What is wrong with this code?
      
### What is the second argument that can optionally be passed to setState and what is its purpose?
     
### What's a pure functional component in React?
     
### What are some recent changes in the React library (e.g. in version 14, 15)?
     
### Why would you need to bind event handlers to "this"?
     
### Why does React use SyntheticEvents?
     
### Why would you use forceUpdate in a React component?
     
### Explain the Virtual DOM concept in React.
     
### If you need to access the underlying DOM node for a React component, what's the typical way to do this in React?
     
### What is the React context?
     
### What is mapStateToProps and mapDispatchToProps?
     
### Which is preferred option with in callback refs and findDOMNode()?
     
### Why are String Refs legacy?
     
### What is React Fiber?
     
### How to create props proxy for HOC component?
     
### How to apply validation on Props in ReactJS?
     
### What are the recommended ways for static type checking?
     
### What is the difference between ReactJS and Angular?
     
### What is the difference between Flow and PropTypes?
     
### What is the difference between using constructor vs getInitialState in React?
     
### When is it important to pass props to super(), and why?
     
### Does React re-render all components and sub components every time setState is called?
     
### How to conditionally add attributes to React components?
     
### Do Hooks replace render props and higher-order components?
     
### How would you go about investigating slow React application rendering?
     
### When would you use StrictMode component in React?
     
### What is Redux Thunk used for?
     
### What is a pure function?
     
### Explain some difference between Flux and AngularJS (1.x) approach
     
### What is React Fiber?
     
### How to use Polymer in ReactJS?
     
### What is reselect and how it works?
     
### How does React renderer work exactly when we call setState?
     
### What is the key architectural difference between a JavaScript library such as React and a JavaScript framework such as Angular?
     
### How to avoid the need for binding in React?