# What is redux? 

Redux is a state management library that implements the flux architecture. 

### When to use redux ?

When you have a large application and have to manage a lot of states in different components. Example:
Imagine a social network as facebook, and then you have a new comment on you're latest picture so not only the comment section
on that picture must be update but also the notification icon.

### Main parts of redux:

- **store**
- **action**
- **dispatch**
- **reducers**

- **What is store?**

    The store is where you will keep your global state. And from where your components will derive the data from (state).

- **What is action?**

    The actions are dispatch with information to our store. They describe the "type" of action we have to take and the payload of it.

- **What is dispatch?**

    Is the kind of "sending" the action to the reducers.

- **What is reducer?**

    Reducers will take our actions, that have been dispatched and update the state in our store.



### Some commons hooks

- **useDispatch()**
- **useSelector()**

- **What the useDispatch hook does ?**

    Taken directly from the redux docs:

    "This hook returns a reference to the dispatch function from the Redux store. You may use it to dispatch actions as needed."

- **What the useSelector hook does ?**

    Taken directly from the redux docs:

    "Allows you to extract data from the Redux store state, using a selector function."



### How to set up redux?

There is a lot of ways. But on common way is to follow this steps:

- 1 Create a folder called redux
- 2 Create inside this folder create another two folders (actions and reducers)
- 3 In the root of your redux folder create a file for your store
- 4 Also, in the root of your redux folder create a actionType
- 5 In your actions folder create your actions (obviously 😸)
- 6 In your reducers folder create your (you've guessed) reducers.
- 7 The boilerplate almost done
- 8 Now in your App file import Provider from react-redux and wrapp around your App component, kinda of like this:

   ```JSX 
   <Provider store={store}>
      <div className="container">
        <h1>My Books</h1>
        <InputSection />
        <div className="line"></div>
        <BooksSection />
      </div>
    </Provider>
   ```
- Now you can import the state from your store whenever you need! 
- If you want more examples check my other repo:
  -  [repo with example](https://github.com/Leonardo-Antunes/Book-CRUD)
 

### References:

- [hooks docs](https://react-redux.js.org/api/hooks)
- [docs redux](https://react-redux.js.org/introduction/getting-started)





