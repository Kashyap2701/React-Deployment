# React-Deployment

This repository contains a React app that demonstrates how to deploy a React app to a live environment and access environment variables.

## Purpose of Development Environemnt

The purpose of a development environment is to provide a dedicated space where developers can build, test, and deploy new software applications or features without affecting the live production environment. This environment is typically set up on local machines or a remote server and is used throughout the software development lifecycle.

## Environment Variables

Environment variables are a way to store configuration information outside of your code. They're commonly used to store sensitive information, such as API keys or database credentials, that you don't want to expose in your codebase. In a Vite React app, you can define environment variables in a `.env` file at the root of your project.

## How to Define and Access Env in Vite React App

To define an environment variable in a Vite React app, create a `.env` file at the root of your project and prefix the variable name with `VITE_` For example, if you wanted to define an API key, you could create a variable called `VITE_API_KEY` in your `.env` file.

To access the environment variable in your app, use the `import.meta.env object`. For example, to access the `VITE_API_KEY` variable, you could use `import.meta.env.VITE_API_KEY` in your code.

## How to Use This App

To use this app, follow these steps:

- Clone this repository to your local machine.
- Install dependencies by running
  ```bash
  npm install
  ```
- Create a `.env` file at the root of your project and define your environment variables like
  ```bash
  VITE_APP_MODE='THIS IS DEVELOPMENT MODE'
  ```
- run your app in development enviornment using
  ```bash
  npm run dev
  ```

## How Structure of Git Branches works in Real Projects

A Git branching strategy that includes "Master," "UAT," "Dev," and "Feature" branches is a common approach to managing software development projects. Here's how this strategy works:

- **Master Branch**: The "master" branch is where you store the production-ready code. This is the branch that you'll deploy to your live environment.

- **UAT Branch**: The "UAT" (user acceptance testing) branch is where you test changes in a staging environment before promoting them to the production environment. This branch helps ensure that new changes and features work as expected and don't introduce regressions or other issues.

- **Dev Branch**: The "dev" branch is where you integrate new features and bug fixes before they're merged into the UAT or master branch. This branch is often used by developers to work on new features or bug fixes independently of other team members.

- **Feature Branch**: The "feature" branch is where developers work on new features or bug fixes. Each new feature or bug fix should have its own branch. This helps ensure that changes can be worked on independently and merged back into the dev branch when they're ready.

![Git-Branching-Strategy](./src/assets/Branching-Strategy.png);
