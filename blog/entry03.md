# Entry 3
##### 02/18/24


## **Context**:

For the freedom project, I have been continuing to learn React for the front end of my group's website. Many of my sources for further learning React since December include but are not limited to [Web dev Developer's video on the useState hook](https://www.youtube.com/watch?v=O6P86uwfdR0&t=559s) and [Web dev Developer's walkthrough on a todo list app](https://www.youtube.com/watch?v=Rh3tobg7hEo).

## **Content**:

While watching the video, I followed along and tried to add some of my own twists to see how the useState hook functions works:

```jsx
    function colorButton() {
    const [state, setState] = useState({count: 0, theme: 'colorless'})
    // output: meant to decrease the value for "count"
    function decreaseCount() {
        setState(prevState => {
             return {...prevState, count: prevState.count -1}
         })
    }
    // output: meant to increase the value for "count"
    function increaseCount() {rt
        setState(prevState => {
            return {...prevState, count: prevState.count +1}
        })
    }

    return (
        <>
        <button onClick={decreaseCount}>-</button>
        <span>{state.count}</span>
        <span>{state.theme}</span>
        <button onClick={increaseCount}>+</button>
        </>
    )
}
```

However, I wanted to do more such as changing the "theme" that is displayed next to the number count. I tried:

```jsx
const [state, setState] = useState({count: 0, theme: 'colorless'})
    // output: meant to decrease the value for "count" and change "theme" into "blue"
    function decreaseCount() {
        setState(prevState => {
             return {count: prevState.count -1 , theme: 'blue'}
         })
    }
    // output: meant to increase the value for "count" and change "theme" into "red"
    function increaseCount() {
        setState(prevState => {
            return {count: prevState.count +1, theme: 'red' }
        })
    }

    return (
        <>
        <button onClick={decreaseCount}>-</button>
        <span>{state.count}</span>
        <span>{state.theme}</span>
        <button onClick={increaseCount}>+</button>
        </>
    )
```

My hypothesis was correct because I thought that by taking out the previous value for the theme and replacing it with another value, the useState function will also change the "theme" and thus it worked out. I tested this conclusion by adding another value into the array for useState:

```jsx
function User() {
    const [state, setState] = useState({count: 0, color: 'colorless', adds: ''})

    function decreaseCount() {
        setState(prevState => {
             return {count: prevState.count -1 , color: 'blue', adds: 'subtracted'}
         })
    }

    function increaseCount() {
        setState(prevState => {
            return {count: prevState.count +1, color: 'red', adds:'added'}
        })
    }

    return (
        <>
        <button onClick={decreaseCount}>-</button>
        <br/>
        <span>{state.count}</span>
        <br/>
        <span>{state.color}</span>
        <br/>
        <span>{state.adds}</span>
        <br/>
        <button onClick={increaseCount}>+</button>
        </>
    )
}
```

This solidifies my idea of changing values in the array of the useState hook and will help contribute to the grading app my team is making. In my array, I changed the number, color, and whether its added/substracted from its previous value.

#### Sources:
* [Web dev Developer's video on the useState hook](https://www.youtube.com/watch?v=O6P86uwfdR0&t=559s)
* [w3schools](https://www.w3schools.com/react/react_usestate.asp)

## **EDP**:

In this entry, I go through the third step of the engineering design process which is brainstorming possible solutions. I have been brainstorming on a viable product where I can use all of what I learned from React to make the grading website I wish to make while combing it with what Yu learned from Firebase with Samuel's help.

## **Skills**:

Throughout this part of my freedom project, I have been teaching myself the skills of **logical reasoning** and **attention to detail**. For instance, in the tinkering above, I thought that it would be logical for adding more values to the array and being able to change it which actually works. With this reasoning, I added the "adds" value to try it out. I also paid close attention to how the video uses syntaxes such as the curly brackets to show values from javascript and the `=>` which was new to me, but I figured out that it was just to help create a new function.

## **Next steps**:

My next steps for the project is to learn the array methods I will need for React and other javascript skills/methods I may need to contribute to my knowledge of React.

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
