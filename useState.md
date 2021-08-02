# useState()

### useState() is a hook that allows you to add state to a functional component. 

So when we create a function and we want state in it we use useState() instead of changing to class syntax.

Ex:

```jsx
const [count, setCount] = useState(0);
```

What happens when we call useState()?

He initialize a variable with state. This will preserve the value, normally the variables disappear after the function is gone, but the variables with state remains.

Wich arguments we pass to useState()?

The initial state.

How do we update the state?

With setState.


References: [useState docs](https://reactjs.org/docs/hooks-state.html)
