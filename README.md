# Presentation

#### 1.1 *React*  
React is a JavaScript Library for Builing User Interfaces.

#### 1.2 *Why do we use React?*  
Because it's Declarative & Composable. React uses One-Way Data Flow, JSX, Virtual DOM, and it's much easier to create mobile apps.    
React makes it easier to create interactive UIs. Design simple views for each state in your application, and React will efficiently update and render just the right components when your data changes.  Declarative views make your code more predictable and easier to debug. React builds encapsulated components that manage their own state, then compose them to make complex UIs. Since component logic is written in JavaScript instead of templates, you can easily pass rich data through your app and keep state out of the DOM. React is the second most popular, if not the most popular JavaScript library after Angular. React  was launched in 2013 and have chosen by the different developers for building user interfaces. React itself is not a complete framework and to provide additional functionlality, developers can use other JS libraries. About 71% of StackOverflow users state that React.js is the best tool and they wish to work on this for their upcoming projects. As per the survey, React.js popularity considerably increased from 2017 to 2019. It is one of the top javascript library and framework. A large number of components, tools and libraries are released to elucidate the developer work and minimise the effort. In every month a new device is made-up to make the react.js more delightful, seamless and fast.  
#### 1.3 *Who Uses React?*   
-Facebook  
-Instagram  
-GitHub  
-WhatsApp  
-Codecademy  
-Netflix  
-PayPal  
-Reddit  
Many big companies like facebook, github, instagram and et cetera(ect) use react in their Apps.  
So let's have a look at the main benefits of the React.  
#### 2.0 JSX
JSX it's a combination Javascript and XML code, more precisely it's a syntax extension to JavaScript. It is similar to a template language, but it has full power of JavaScript. JSX gets compiled to React.createElement() calls which return plain JavaScript objects called “React elements”.  
Let's look at the syntax.

#### 2.1 SYNTAX
There is a JavaScript example and a JSX, and JSX probably looks better.  

#### 3.0 Virtual Document Object Model  
The virtual DOM is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM.  

#### 3.1 Shadow DOM !== Virtual DOM
The VirtualDOM isn't the shadowDom, do not confuse.  
The Shadow DOM is a browser technology designed primarily for scoping variables and CSS in web components. The virtual DOM is a concept implemented by libraries in JavaScript on top of browser APIs.  

#### 3.2 Two basic steps to re-render  
There are two basic steps to re-render our App.
Actually re-rendering the entire app on each change only works for the most trivial apps. In a real-world app, it's prohibitively costly in terms of performance. React has optimizations which create the appearance of whole app re-rendering while maintaining great performance. The bulk of these optimizations are part of a process called reconciliation.  
Reconciliation it's an algorithm which React uses to diff one tree with another to determine which parts need to be changed. Usually the result of `setState React function' eventually results in a re-render our App. The central idea of React's API is to think of updates as if they cause the entire app to re-render. A high-level description goes something like this: when you render a React application, a tree of nodes that describes the app is generated and saved in memory. This tree is then flushed to the rendering environment — for example, in the case of a browser application, it's translated to a set of DOM operations. When the app is updated, a new tree is generated. The new tree is diffed with the previous tree to compute which operations are needed to update the rendered app. React is designed so that reconciliation and rendering are separate phases. The reconciler does the work of computing which parts of a tree have changed. The renderer then uses that information to actually update the rendered app.  

#### 3.3 Result  
Here we can see our result.  
The Virtual DOM will only update what is necessary.  

#### 4.0 Components  
React components are small, reusable pieces of code that return a React element to be rendered to the page. The simplest version of React component is a plain JavaScript function that returns a React element.

#### 4.1 Components  
Components can also be ES6 classes or arrow functions.

#### 4.2 Components  
Components can be broken down into distinct pieces of functionality and used within other components. Components can return other components, arrays, strings and numbers. A good rule of thumb is that if a part of your UI is used several times (Button, Panel, Avatar)
or is complex enough on its own (App, FeedStory, Comment) it is a good candidate to be a reusable component.  

#### 4.3 Components life cycle
Let's look at the three basic Components life cycles.  
-componentDidMount() is invoked immediately after a component is mounted (inserted into the tree). Initialization that requires DOM nodes should go here. If you need to load data from a remote endpoint, this is a good place to instantiate the network request.  
-componentDidUpdate() is invoked immediately after updating occurs. Use this as an opportunity to operate on the DOM when the component has been updated. This is also a good place to do network requests as long as you compare the current props to previous props (for example a network request may not be necessary if the props have not changed).   
-componentWillUnmount() is invoked immediately before a component is unmounted and destroyed. Perform any necessary cleanup in this method, such as invalidating timers, canceling network requests, or cleaning up any subscriptions that were created in componentDidMount().

#### 4.3 ReactDOM.render()
We need to use ReactDOM.render to render the components on he page.  
ReactDOM.render creates the component, starts the framework, and injects HTML into a DOM node.  

#### 5.1 Props  
Normally you start out with React JSX syntax for rendering something to the browser when learning about React.   

#### 5.2 Props  
Pretty soon you will split out your first React component.  
A common question followed by this act: how to pass the data as parameters from one React component to another component?   
That's because you don't want to have a component rendering static data, but pass dynamic data to your component instead. 
That's where React's props come into play. You can pass data in React by defining custom HTML attributes to which you assign your data with JSX syntax. React props are only passed from top to bottom in React's component tree. There is no way to pass props up to a parent component.  In addition, it's important to know that React's props are read only. Passing only props from component to component doesn't make the component interactive, because nothing is there to change the props. That's the time when React state comes into play.
A component needs state when some data associated with it changes over time. For example, a Checkbox component might need isChecked in its state, and a NewsFeed component might want to keep track of fetchedPosts in its state. The child component doesn't know whether the incoming props are state or props from the parent component. The component just consumes the data as props. 
And the child component re-renders too once the incoming props changed.

#### 5.3 State  
In this case, the code uses a ternary operator to either show the greeting or not.  The state makes the React components interactive. 
You can read and write state, whereas props are read-only. Once the state changes, the component renders again. In conclusion, every time the props or state change, the rendering mechanism of the affected component is triggered. That's how the whole component tree becomes interactive.

#### 6.0 Thank you for attention!
That's all, thank you for your attention, bye!

