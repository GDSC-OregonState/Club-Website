---
title: "React"
description: "Learn React Web Development"
coverImage: "/react.png"
category: "Tools"
inDev: False
pubDate: "2025-11-3"
updatedDate: ""
publishDate: "Nov 3rd"
---

# React User Interfaces

**React** is a JavaScript library for building user interfaces (UIs), which are the parts of an application that users see and interact with. Think of it as a powerful toolkit for creating interactive and dynamic web pages. Instead of building a whole webpage as one giant piece, React lets you break it down into small, manageable, and reusable pieces. It's currently one of the most popular tools for front-end web development.

-----

## Core Concepts

Understanding these ideas is key to using React effectively.
 - **Components:** Reusable UI building blocks, like custom HTML tags (e.g., <Button>, <ProfileCard>).
 - **JSX:** A syntax that lets you write HTML-like code directly in your JavaScript.
 - **State:** Data that a component manages internally. When state changes, the component re-renders itself.
 - **Virtual DOM:** A lightweight copy of the webpage. React updates this first, then efficiently updates only the changed parts of the real screen.
 - **Props (Properties):** Data passed down from a parent component to a child component to customize it. Props cannot be changed by the child.
 - **One-Way Data Flow:** Data flows in one direction (parent to child), which makes your app's behavior more predictable and easier to debug.
 - **Hooks:** Special functions (like useState or useEffect) that let you "hook into" React features, like state, from your functional components.

-----

### Setup Guide

1.  **Download and Install Node.js**

    * React projects require **Node.js** and its package manager, **npm**.
    * Go to [https://nodejs.org/](https://nodejs.org/)
    * Download the installer for your operating system. The **LTS (Long Term Support)** version is recommended.
    * Run the installer. `npm` is included automatically.

2.  **Check Your Installation**

    * Open a terminal (or Command Prompt).
    * Verify that Node.js and npm are installed by checking their versions.

    ```bash
    node -v
    npm -v
    ```

3.  **Create Your React App**

    * You don't install React globally. Instead, you use a tool to create a new project folder.
    * The `npx` command (included with npm) runs the official tool to create a new React app.
    * Replace `"my-app"` with the desired name for your project folder.

    ```bash
    npx create-react-app my-app
    ```

4.  **Run Your New App**

    * Once it's finished, navigate into your new project directory.
    * Start the development server.

    ```bash
    cd my-app
    npm start
    ```

    * This will automatically open your new React app in your default web browser (usually at `http://localhost:3000`).

-----

## React Challenges

### Easy

1.  **Customize the Starter Page** (25 pts)
    * In `App.js`, find the `<header>` section.
    * Change the text inside the `<p>` tag to "My first React app!"
    * Add a new `<h2>` tag directly below the `<p>` tag that contains your name.

### Medium

2.  **Create a Live Text Mirror** (50 pts)
    * Use the `useState` hook to create a state variable called `inputText`, initialized to an empty string.
    * Create an `<input type="text">` element.
    * Make this a "controlled component" by setting its `value` to your `inputText` state and using its `onChange` event to update the `inputText` state.
    * Below the input, add an `<h2>` tag that displays the `inputText` state live as the user types.
    * Add a "Reset" button that, when clicked, sets the `inputText` state back to an empty string.

3.  **Build a Reusable `UserCard` Component** (75 pts)
    * Create a new component file (e.g., `UserCard.js`).
    * This component should accept `name` and `imageUrl` as **props**.
    * Inside the component, display the `name` in an `<h3>` tag and the `imageUrl` in an `<img>` tag.
    * Add some simple inline CSS styling to give the card a border, padding, and a set width.
    * Import and use your `<UserCard>` component at least three times in `App.js`, passing in different names and image URLs for each.


### Hard

4. **Build a To-Do List Page** (125 pts)
    * Use both `useState` and reusable components to create a to-do list page with tasks that you can check off.
    * Create an `<input type="text">` element and a submit button to create a new to-do item and add it to a `useState` list.
    * Update the list of visible items with new to-do items.
    * Create a to-do item component that can be created for each item in the list.
    * Make it so you can check off items and they will be removed from the to-do list.

-----

## 🔗 Resources to Get Started
- [React Official Docs](https://react.dev/learn)
- [Vite (Modern React Project Starter)](https://vite.dev/guide/)
- [React Router (Routing Library)](https://reactrouter.com/)
- [Redux (State Management Library)](https://redux.js.org/)
- [MUI (React UI Component Library)](https://mui.com/)

-----

## 🔗 How to Submit
1. For the your submissions, share your project repository or a screenshot/video.

Submission Form: [Submit Here](https://forms.gle/g3TbxaU2r4sCy84XA)