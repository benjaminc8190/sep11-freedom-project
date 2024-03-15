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
 * `let num = prompt("what is your favorite number?")`
 * will input the value into  `<h1>{hello + num}</h1>`(This is a string concactenation because hello is a different variable)

1/8/24
*[Youtube video on hooks](https://www.youtube.com/watch?v=O6P86uwfdR0&t=559s)*
* Learned about when you cannot use hooks
    * `useState` - returns an array with the value of its current state and a value of a function to update it

1/23/24
*[Youtube video on a project](https://www.youtube.com/watch?v=Rh3tobg7hEo)*
* New mindset for integrating to React-
    * Think of JS as instructions to make a sandwich while React is going to a store for the same sandwich; JS is more Imperative while React is more declarative.
* General format for each file- Hooks, helper functions, reuturn functions
    * Hooks are generally used on top of the function
* `useEffect` - Runs a function everytime the value of the array changes

2/1/24
*[Youtube video on knowledge I need for React](https://www.youtube.com/watch?v=JR9wsVYp8RQ&t=169s)*
* Checklist of things from js I will need for React when moving forward:
    * Scoping
    * Callbacks
    * Passing functions to other functions
    * Array methods-
        * math()
        * sort()
        * filter()
* Video includes a link to a more detailed [checklist](https://javascriptsimplified.com/beginner-table-of-contents/)

3/1/24
*[Youtube video on connecting React with Firebase](https://www.youtube.com/watch?v=ad6IavyAHsQ)*
* import method for "firebase" from firebasefile
* import addDoc,collection from @firebase/firestone
* To get a value from the collection, you must make a var equal to collection

3/7/24
*Went through the project that a partner has created and started*
I searched up the codes up when I didn't understand, or just simply asked
* Flexbox (basically used to replace Bootstrap's column feature) for css [source](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* Routing multiple pages for React [source](https://www.w3schools.com/react/react_router.asp)
* Interloping is best practice for inserting variables easily
* Experienced how it feels like to have to solve a merge conflict

3/15/24
*[Installing Firebase to React Project](https://www.youtube.com/watch?v=_KN_eCnZgOA)*
* Aha moment: I was supposed npm install firebase outside of the react folder. When I installed firebase inside of the React app folder, the terminal displayed an error of vulnerablilities. I followed the video on installing firebase in the ide before the React app folder and there were no vulnerablilities.
* The video also showed how to initialize firebase
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
