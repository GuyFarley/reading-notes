# Code 301 - Class 04 - React and Forms

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

### What is a ‘Controlled Component’?

- An input form element whose value is controlled by React. In these components, React is "the single source of truth"

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why

- We should update the state with their responses as soon as they enter them. This is because we may want to do something with that data as soon as it's entered, rather than waiting for the entire form to be submitted
- For example, we may want to log the user's name as soon as they enter it into the form

### How do we target what the user is entering if we have an event handler on an input field?

- We would have the event handler call a function that targets the value being entered into the field, and change the component's state
- This will also re-render the component as the information is entered by the user
- Example (from the React article linked above):

```
class EssayForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      value: 'Please write an essay about your favorite DOM element.'
    };

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('An essay was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Essay:
          <textarea value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}
```

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

### Why would we use a ternary operator?

- It saves a lot of unnecessary typing to achieve the same result as an if statement, for testing conditions

### Rewrite the following statement using a ternary statement

```
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Ternary version:

```
x === y ? console.log(true) : console.log(false)
```

[Back to Home](../README.md)
