---
layout: post
title:      "The Finale of All Finales...sort of... "
date:       2020-12-09 22:12:38 +0000
permalink:  the_finale_of_all_finales_sort_of
---


Well...the month has finally come. I am down to my last project at Flatiron. I have decided to build an application that would tie in my current career industry, legal, to software engineer - a case and document management system. I used rails for my backend and react/redux for the frontend. Keep in mind that I plan to add to this app. 

In my backend, I have my Matter Model and Task Model - a matter has many tasks and a task belongs to a matter. The frontend is built with react and redux. React is a framework built entirely out of Javascript. There are components, props, and states that were introduced. After several weeks of learning React, we dive into Redux. Redux is an open-source JavaScript library for managing application state.  

To build my React app, I first type in my command line `npx create-react-app app-name`. This command line tool from Facebook allows you to generate a new React project and use a pre-configured webpack build for development. It will set up the following project structure:

```
new-app
├── .gitignore
├── node_modules
├── package.json
├── public
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── README.md
├── src
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
└── yarn.lock
```

Some advantages and limitations of ReactJS are:

**Advantages**:
* Free and open source
* highly adaptable
* Virtual DOM makes it extremely efficient
* JSX increases fode reliability and makes mixing HTML and JS much easier
* Makes UI testing easier
* Developer tools such as the React.js chrome extension for debugging
* Lare supporting community

**Limitations**:
* It is a library, not a framework. It handles the UI only. You need to use other libraries for other parts of your app.
* No set way to structure applications, meaning you have to figure it out for yourself.
* Its flexibility can easily let developers make poor choices
* JSX and inline templating can make the code quite complex.

**What are React's key features?**
* Virtual DOM
* JSX
* Unidirectional Data Flow
* Server-Side Rendering

# REDUX
Redux is a popular library in today's marketplace. It is used to manage the application's state. It is widely used because it allows you to pass data without the need to pass props through every level (aka props drilling). The main constituents of Redux are Actions, Reducers, and Store.

Since redux is all about the state, how does one change state? The only way to update a state is to dispatch, or trigger, an action. An action is just plain JavaScript object to describe the action taking place. 

When reviewing redux concepts, I really like this image describing the flow of the main constituents in Redux:

![](https://redux.js.org/assets/images/ReduxDataFlowDiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif)

I think it does a good job encapsulating what is happening. 





