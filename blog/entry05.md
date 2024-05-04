# Entry 5
##### 5/1/24

## **Minimum Viable Product**:

The MVP, the bear-bones of our [website](https://ricegrades.pages.dev/), is finished - my partners and I have been working on it throughout April to get our grading website to work. There, however, are still some improvements that can be made such as making the student and teachers look better by fitting the theme of our website rather than black and white blobs of texts. We are also thinking of making an assignments system so that the teacher can name the assignments rather than just typing in a grade for the students.

Throughout the Spring break, Yu, Samuel, and I have been calling each in a group chat where Yu and I acted as navigators while Samuel worked on the code. We offered ideas on what the teachers should see when they log in. Such as seeing the classes they made, making classes, and allocating the weight of each section of grades(Ex: summative assignments). I have to give credit to Samuel for coming up with the complicated js code such as `Promise((resolve, reject)`.

## **Tool**:

As we have been completing the MVP, I continued to learn my tool through some more [Freecodecamp](https://www.freecodecamp.org/learn/front-end-development-libraries/#react) lessons. I have been learning about props, proptypes, and stateless vs stateful functions throughout these lessons.

Along the challenges of Freecodecamp, I have encountered many mistakes that helped me understand the concepts better. For example, I tried to get the `Items` component to require that `quantity` to be a number using `propType` defining. From the exmaple, I started with `Items.propTypes = {handleClick: PropTypes.quantity.isRequired}`. This only would've worked if I was checking a click, but in this situation, I am only checking the function `Items`. I also needed to make sure that I am checking the whether the given `quantity` was a number not the other way around because this is reading that `quantity` is required. So, I wrote `Items.propTypes = { quantity: PropTypes.number.isRequired};`. That's why I need to pay attention to what variable I am checking for and what's required for the input of the variable.

I also played around with the stateful functions that I got from Freecodecamp on [Stack Blitz](https://stackblitz.com/edit/af-react-sandbox?file=index.js).

I started with the following which displays "Initial State" orginally then displays "React Rocks" after a button is clicked:

```jsx
constructor() {
    super();
    this.state = {
      name: 'Initial State'

    };
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
    this.setState({
      name: 'React Rocks'
    });
  }

  render() {
    return (
      <div>
        <h1>{this.state.name}!</h1>

        <button onClick={this.handleClick}>Click Me</button>
      </div>
    );
  }
}
```

I thought it would be cool if I can revert the value back to what it was before such as changing "React Rocks" back to "Initial State". I tried to search up how I would revert the value of the new state(after clicking the button) back into its initial state(before clicking the button), but unfortunately, I read that it isn't a built-in way to do so on (stack overflow)[https://stackoverflow.com/questions/54895883/reset-to-initial-state-with-react-hooks] so I  asked ai to help me. I kept asking it questions on new things that I have never seen before such as `...` and a little bit of how `Object.assign({})` works. I recorded these new js methods in my notes as to how they work.

```jsx
class App extends Component {
  constructor() {
    super();
    this.initialState = {
      name: 'Initial State',
    };
    // Set the initial state using object spread syntax
    this.state = Object.assign({}, this.initialState);

    this.handleClick = this.handleClick.bind(this);
    this.handleReset = this.handleReset.bind(this);
  }

  handleClick() {
    this.setState({
      name: 'React Rocks',
    });
  }//updates the name to React Rocks

  handleReset() {
    this.setState({ ...this.initialState });
  }//sets the name back to initial

  render() {
    return (
      <div>
        <h1>{this.state.name}!</h1>
        <button onClick={this.handleClick}>Click Me</button>
        <button onClick={this.handleReset}>Reset</button> {/* Reset button */}
      </div>
    );
  }
}
```


## **EDP**:

This is the fifth step of the engineering design process. Our MVP is the prototype of our project because it is functioning the way we want it to. We are testing by making alternate accounts to view the teacher and student pages to see what improvements need to be made such as adding css to make the pages look better. We are also looking for pictures to put on the homepage of our website.

## **Skills**:

Throughout this part of the project, I have continued to develop the skills such as **attention to detail** and **How to read.** For example, I paid attention on how `Object.assign({}, this.initialState)` was used by the ai to help me with js. I also read through the blurs that freecodecamp has on the left side above the directions to learn about a concept before doing it. For example, I started out with their example that was given when I tried to get a proptype required(the first example of how I learned from Freecodecamp above).

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
