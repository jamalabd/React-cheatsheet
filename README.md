# React-cheatsheet
Creating this as a resource for future me and other developers who just need a refresher or even for beginner React learners. This is meant to be simple to understand & easy to read.

As always any contributions will be much appreciated!

## What is React ⚛ ? 
React is a JavaScript library for rendering user interfaces (UI). UI is built from small units like buttons, text, and images. React lets you combine them into reusable, nestable components.

Now that we got that out the way let's dive straight into it.

## Virtual DOM vs DOM 📄
DOM The DOM stands for Document Object Model. It is an Object Model of the Document or a Model of the Objects that make up the Document. Doesnt matters how you slice the bread as long as it's eatable 🍞. 

No matter the browser you use they will all create a DOM for the webpage you are on ( for the resource you are trying to access, for the location you are trying to reach, etc..).


It will create this DOM in a tree-like structure. Containing HTML elements and each element's events, properties, and methods.
<!--Todo insirt crappy drawing-->

Whenever there is a change to some content in the DOM ( the state of the DOM changes ) the entire DOM will be repainted or rerendered to apply those new changes.

The Virtual DOM is a virtual copy of the DOM. When our applications state changes it first updates the virtual DOM. Figures out exactly what has changed using reacts diffing algorithm comparing the real DOM and the Virtual one and finding the best way to make these changes. This is what makes react high performante. 



![lnrn_0201](https://github.com/jamalabd/React-cheatsheet/assets/45414121/981c8e90-af0e-4eba-90cc-f256bd9a515d)

## What is JSX? 🙅🏾‍♂️
JSX stands for Javascript in XML ( eXtensible Markup Language ), like HTML ( Hypertext Markup Language ) XML is a highly readable markup language. So essentially JSX is Javascript written to look like HTML.

The key here is to remember 'looks like'. We are not actually writing any HTML, JSX gives us the readability of HTML while leveraging the functionality of Javascript. JSX is used to describe what the UI will look like. In this way react is [Declarative](https://alexsidorenko.com/blog/react-is-declarative-what-does-it-mean/).

So why JSX? Essentially JSX allows us to combine our markup and our logic. This gives us the ability to keep our markup and our logic for let's say a header component in the same file. 

## Class components vs Functional components 🎻 🆚 🧮
Before we get into the difference between Class-based components and function-based components it's important to know what a component is in react. 
A component is simply a way of organizing your code. Components are written in JSX and JSX is used to describe what the UI will look like so each component will describe a peace of the UI. 

This allows you to split up your code into reusable pieces that you can use throughout your application, it also has the added benefit of forcing you to focus on one piece of UI at a time, thinking of each piece in isolation. Each component will return a JSX element.

Currently, it is not very common to see organizations still using class-based components since functional have hooks ( more on this later ).

### Class Component example
```javascript
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```
### Functional component example
```javascript
function Welcome(props) {
  return (
    <h1>Hello, {props.name}</h1>;
  )
}
```

## Props 💁🏽‍♂️
### What are props???
Before answering that it's important to know how data flows or is transferred in React. Unlike Angular where data can flow from parent 
( top ) to child ( bottom ) and from child to parent in React data only flows one way, Down.

From parent to child. We call this unidirectional data flow 🪄. Your data only flows/moves in one direction. There are ways around this but at its core, this is how React was designed to be used

Now props are short for properties ( but you didn't hear that from me 🤐 ).
<!-- 
--Todo--
## Hooks
### Use callback 📞
Not going to lie this one had me stumped when it first came out 😅.

use callback is a React Hook that lets you save a function that you have already defined between re-renders -->
