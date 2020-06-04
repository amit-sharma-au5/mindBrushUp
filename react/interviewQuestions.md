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

  
### How would you prevent a component from rendering?
     
### What does "shouldComponentUpdate" do and why is it important?
     
### What is JSX?
     
### What is equivalent of the following using React.createElement?
  
### What is a store in redux?
     
### What is an action?
  
### What don't you like about React?
  
### What can you tell me about JSX?
     
### Name some popular Flux Libraries
     
### What are stateless components?
     
### Given the code defined above, can you identify two problems?
      
### What is the difference between createElement and cloneElement?
     
### What's the difference between a "smart" component and a "dumb" component?
     
### What is the render method for?
     
### What are some limitations of things you shouldn't do in the component's render method?
     
### What's an alternative way to avoid having to bind to this in event callback methods?
     
### What is the point of using keys in React?
     
### What's the typical pattern for rendering a list of components from an array of data?
     
### What is reconciliation in React?
     
### What's the difference between an Element and a Component in React?
     
### What is the point of shouldComponentUpdate() method?
     
### What are PropTypes in React?
     
### What is ReactDOM?
     
### What are typical middleware choices for handling asynchronous calls in Redux?
     
### What's the typical flow of data like in a React + Redux app?
     
### What are Pure Components?
     
### Why should not we update the state directly?
     
### What is the difference between HTML and React event handling?
     
### How to bind methods or event handlers in JSX callbacks?
     
### What are synthetic events in ReactJS?
     
### What is Key and benefit of using it in lists?
     
### What are forward refs?
     
### What is the difference between ShadowDOM and VirtualDOM?
     
### What are uncontrolled components?
     
### What is the difference between createElement and cloneElement?
     
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