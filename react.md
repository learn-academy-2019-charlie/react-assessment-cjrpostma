# React Assessments
Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React is a modern, efficient answer to complex UI applications
- React is a flexible library that plays the role of V in an MVC framework

 
#### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.
//Your Answer
- Smart components include state.
- Dumb components do not include state however they may consume state.
- The distinction helps better organize state to the correct place, typically higher in the state tree of the application. It therefore also allows us to see which components are altering state and which are consuming it.

//Googled Answer
- Smart components keep track of state.
- Dumb components render.
- Using the container design pattern, the container components are separated from the presentational components and each handles their own side of things. The container components do the heavy lifting and pass the data down to the presentational components as props.


#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?
//Your Answer
 - Installs dependencies. Updates package.json.

//Googled Answer
 - npm and Yarn are two well-known JavaScript package managers. If you’re not familiar with what a package manager does, it essentially is a way automate the process of installing, updating, configuring, and removing pieces of software (AKA packages) retrieved from a global registry.

#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

    import React, { Component } from 'react';

    class Recipes extends Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:
          [
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}
          ]  
        }
      }

      render() {
    
        return (
    
          let recipes = this.state.recipes
          
          recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })
    
          <ul>
            {recipes}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)
 
//Your Answer
 - email
 - textarea
 - number
 - password

//Googled Answer
 - <input type="button">
 - <input type="checkbox">
 - <input type="color">
 - <input type="date">
 - <input type="datetime-local">
 - <input type="email">
 - <input type="file">
 - <input type="hidden">
 - <input type="image">
 - <input type="month">
 - <input type="number">
 - <input type="password">
 - <input type="radio">
 - <input type="range">
 - <input type="reset">
 - <input type="search">
 - <input type="submit">
 - <input type="tel">
 - <input type="text">
 - <input type="time">
 - <input type="url">
 - <input type="week">

#### 7. How would you explain state to a friend who doesn't know code?
//Your Answer
 - State is a snapshot in time of the current value of any number of parameters.

//Googled Answer
 - State is a JavaScript object that stores a component’s dynamic data and determines the component’s behaviour. Because state is dynamic, it enables a component to keep track of changing information in between renders and for it to be dynamic and interactive. State can only be used within a class component. If you anticipate that a component will need to manage state, it should be created as a class component and not a functional one.

#### 8. What is the difference between component state and props? Your answer should include a short explanation of both.
//Your Answer
 - Component state: the dynamic properties of the state object that exist in a smart component and that can be updated using the setState() method. The current state can be sent to other components as props.
 - Component props (properties): the properties that are passed down from a stateful component for use in child components.

//Googled Answer
  - In a React component, props are variables passed to it by its parent component. State on the other hand is still variables, but directly initialized and managed by the component.

#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.

 - The greatest challenge I experienced during this activity was learning to effectively pair program. My partner was more advanced than me and I needed to learn how to communicate that I was still attempting to grasp the solution to the usecase at hand before moving to the next usecase. I also learned how to better walk through my thoughts outloud as a way of explaining my problem solving approach. I gained empathy towards future pairing partners where I am the one thinking faster about particular topics and how to slow myself and make the experience useful for both partners.