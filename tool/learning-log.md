# Tool Learning Log

Tool: **React**

Project: **Grading website**

---

10/23/23:
*Samuel's tutorial in the library*-
* Start with downloading a folder : `npx create-react-app appName(folder)`
* All cdn should go in the `public/index.html` folder
* Files not needed(deleted):  reportWebVitals, setupTests, logo.svg, App.test.js, index.css

10/27/23:
*[Free code camp](https://www.freecodecamp.org/)*-
* jsx is an extension that lets you use html in js
* JSX must return a single element of html
* To transpile several JSX elements, you must put them in a parent(div)
* To comment in JSX, use `{/* */}`

10/28/23:
*Mini Project*-
* Must use capital letters as first letter for files that contain components
* import/export functions into App.js from other files
* Reusable functions were used as reusable components from Bootstrap

11/06/23
*[Free code camp](https://www.freecodecamp.org/)*-
* ES6 method for making a component
* Composing child component into parent components

11/13/23
*[Tic Tac Toe project by React](https://react.dev/learn/tutorial-tic-tac-toe)*-
* Making buttons a function(component) and plugging it into a another function to create a row(Bootstrap component)
* assigning classes for the element will be `className ="class"`
    * Tried to assign a class, standard, into the h1 tag to change its font size to fit `<h1 class="standard"> Hello World</h1>` and found out that it will not work because I used `class` instead of `className`.

11/14/23
*Continuation from 11/13*
* To escape back into javascript, use curly bracket {}
* onClick is a method that lets the user click on an element for something to happen `onClick={action}`
* I learned to allow user interactivity by `setValue('X');` so when the user clicks the button, it will display X.

11/18/23
*[React tutorial by Mosh](https://www.youtube.com/watch?v=SqcY0GlETPk)*
* Pascal casing importance
* Use variables in elements by escaping with `{}`
    * Tried to input the values of hello and num into an h1 element by `<h1>{hello + num}</h1>`
* `return` mulitple lines with `()`
* `.map()` helps in react rendering by creating new array for key properties
* jsx fragments

11/20/23
*Mini project continuation from 10/28*
* Import/export images into and from functions
    * And put it into a Carousel(bootsrap component)
* Add navbar component
* input defined variables into the components

12/4/23
*Continued mini project of 10/28*
* Added user interactivity by letting them answer a prompt
 * l`et num = prompt("what is your favorite number?")`
 * will input the value into  `<h1>{hello + num}</h1>`(This is a string concactenation because hello is a different variable)



<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
