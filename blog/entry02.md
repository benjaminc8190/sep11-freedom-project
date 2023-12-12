# Entry 2
##### 12/11/23

## **Context**:

In order to learn my tool for the freedom project, watching tutorials and doing projects based on React documents throughout the month of November. I used many sources such as [React's tic tac toe game](https://react.dev/learn/tutorial-tic-tac-toe), [React tutorial by Mosh](https://www.youtube.com/watch?v=SqcY0GlETPk), and even [Freecodecamp](https://www.freecodecamp.org/).

## **Content**:

#### Source #1: [Tic Tac Toe project by React](https://react.dev/learn/tutorial-tic-tac-toe)

In this tutorial, it premade the classes with css when I forked its document. I tried to assign the class they wanted "square", but I assigned it like this:

```jsx
function Square({ value, onSquareClick }) {
  return (
    <button class="square" onClick={onSquareClick}>
      {value}
    </button>
  );
}
```

I was confused on why the square was not showing, but when I read on the tutorial, I saw that they assigned the class by `className` because class was already a keyword in Javascript. Like this:

```jsx
function Square({ value, onSquareClick }) {
  return (
    <button className="square" onClick={onSquareClick}>
      {value}
    </button>
  );
}
```

#### Source #2: [React tutorial by Mosh](https://www.youtube.com/watch?v=SqcY0GlETPk)

While watching the tutorial, I followed along as I created my own code where I learned to input values into html:

```jsx
  let num = prompt("what is your favorite number?")
  let hello = "Hi there"
  return (
    <div>

      {/* Navbar */}
      <Navbar />
      {/* first */}
      <h1>hello + num</h1>
      <Para />
  );
```

I had a misconception about brackets becuase I didn't think I'd need it, but I saw that there was no value but "hello + num"(which was what I didn't want), so I added brackets after watching that Mosh has put brackets in his values that he defined with javascript.

```jsx
  let num = prompt("what is your favorite number?")
  let hello = "Hi there"
  return (
    <div>

      {/* Navbar */}
      <Navbar />
      {/* first */}
      <h1>{hello + num}</h1>
      <Para />
  );
```

## **EDP**:

In this entry, I went through the second step of the engineering design process which is researching. The sources were what I used to research my tool to learn how to use it. The next step is to brainstorm ideas with my partners about how we'll be using the tools we individually researched for the freedom project.


## **Skills**:

Throughout the month of researching my tool, I have been working on **self-planning** and **embracing failure**. I had many failures when making a project, but I made sure that I have enough time to process and learn from the mistakes I made. For example,I planned ahead of time about when to do some activities and when I will have time to process them. I delegated Mondays to look through the documents or watch videos then on Tuesdays I review it and record what I learned. Then on Fridays, I review everything and wrote down the proper syntax and concepts in my notes. Through this, I also embraced the mistakes I've made such as the misconception about the bracket around javascript values from above, I recorded in my notes that javascript values must be in bracets. I also recorded in my notes about the `className` syntax.


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
