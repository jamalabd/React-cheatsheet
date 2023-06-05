# React-cheatsheet
Creating this as a resource for future me and other developers who just need a refresher or even for beginner React learners. This is meant to be simple to understand & easy to read.

As always any contributions will be much appreciated!

## What is React ⚛ ? 
React is a JavaScript library for rendering user interfaces (UI). UI is built from small units like buttons, text, and images. React lets you combine them into reusable, nestable components.

Now that we got that out the way let's dive straight into it.

## Virtual DOM vs DOM
DOM The DOM stands for Document Object Model. It is an Object Model of the Document or a Model of the Objects that make up the Document. Doesnt matters how you slice the bread as long as it's eatable 🍞. 

No matter the browser you use they will all create a DOM for the webpage you are on ( for the resource you are trying to access, for the location you are trying to reach, etc..).


It will create this DOM in a tree-like structure. Containing HTML elements and each element's events, properties, and methods.
<!--Todo insirt crappy drawing-->

Whenever there is a change to some content in the DOM ( the state of the DOM changes ) the entire DOM will be repainted or rerendered to apply those new changes.

The Virtual DOM is a virtual copy of the DOM. When our applications state changes it first updates the virtual DOM. Figures out exactly what has changed using reacts diffing algorithm comparing the real DOM and the Virtual one and finding the best way to make these changes. This is what makes react high performante. 



![lnrn_0201](https://github.com/jamalabd/React-cheatsheet/assets/45414121/981c8e90-af0e-4eba-90cc-f256bd9a515d)


<!-- 
--Todo--
## Hooks
### Use callback 📞
Not going to lie this one had me stumped when it first came out 😅.

use callback is a React Hook that lets you save a function that you have already defined between re-renders -->
