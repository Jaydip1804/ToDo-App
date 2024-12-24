# Todo List App

## Welcome! 👋

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [How to setup the project](#how-to-setup-the-project)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Manage your tasks efficiently with our interactive Todo List app! 

This user-friendly frontend application allows users to:-
- View the optimal layout for the app depending on their device's screen size.
- See hover states for all interactive elements on the page.
- Perform various actions such as adding new todos to the list.
- Marking todos as complete, deleting todos, filtering todos by all/active/complete status, clearing all completed todos, and toggling between light and dark mode.
- As a bonus feature, users can also drag and drop to reorder items on the list.

### How to setup the project

To set up the project locally, follow these steps:

1. Clone the repository using GitHub Desktop or Git Bash:
    ```bash
    git clone https:https://github.com/Jaydip1804/ToDo-App/edit/main/README.md
    ```
2. Open the project folder in your code editor.
3. Run the project using a live server extension or deploy it using Netlify, Vercel, or another web hosting and deployment service.

### Screenshot

![Design Preview](./design/active-states-dark.jpg)

### Links
- Live Site URL: [Live Site](https://jaydip1804.github.io/ToDo-App/)

## My process

### Built with

- HTML5
- CSS3
- JavaScript

You will find all the required assets in the `/design` folder. The assets are already optimized.

There is also a `style-guide.md` file containing the information you'll need, such as color palette and fonts.

### What I learned

This project has been a great teacher of implementing CRUD operations in a web app which can be implemented with any tech stack of your choice as underlying logic is same as shown-

```js
function removeTodo(e) {
  if (e.target.nodeName !== "IMG") return;
  const removedItem =
    e.target.parentNode.previousElementSibling.children[2].textContent;
  todoArray = todoArray.filter((todo) => {
    if (todo.todoItem !== removedItem) return todo;
  });

  if (window.confirm(`Are you sure you want to delete: ${removedItem}`)) {
    e.target.parentNode.parentNode.remove();
    handleEmptyMessage();
    getTodoCount();
  } else return;
  saveToLocalStorage(todoArray);
}
```

### Continued development

The continuously learning journey of a programmer never ends. This project made me realize that there are many concepts that I need to work upon including fundamentals like flex-box and its properties, to more complex concepts like working with fetch and async await in javascript. These areas are some that I think I need to work more upon in the upcoming future as they highlight some of the most significant regions of web development that are important for every developer to know of. 

These key points mentioned here will help me grow accountable and consistent towards improving at writing good quality code and be a successful full stack developer one day.


## Author

<b><strong>Jaydip Pawar</strong></b>


## Acknowledgments

I feel like the solutions provided on the website and the continuous doubt solving by industry experts on discord for free is something that is unmatched by anyone else and need to be acknowledged for their efforts in improving me as a developer by suggesting the best practices in your respective tech stack.

## Got feedback for me?

I love receiving feedback! I am always looking to improve my code and take up new innovative ideas to work upon. So if you have anything you'd like to mention, please email 'hi' at saarsaach30[at]gmail[dot]com.

If you liked this project make sure to spread the word and share it with all your friends.

**Stay organized and productive!** 📝✅
