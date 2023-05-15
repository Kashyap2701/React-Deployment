# React-Deployment

This repository contains a React app that demonstrates how to deploy a React app to a live environment and access environment variables.

## Purpose of Staging Build

When deploying a React app, it's common to have multiple environments, such as development, staging, and production. The staging build is a version of the app that's deployed to a staging environment for testing before it's deployed to production.

Link : https://gleeful-souffle-096d93.netlify.app/

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
  VITE_APP_MODE='THIS IS STAGING MODE'
  ```
- Build the app for staging by running
  ```bash
  npm run build
  ```
- Serve the app in staging mode by running
  ```bash
  npm run serve
  ```

## How Structure of Git Branches works in Real Projects

![Git-Branching-Strategy](./src/assets/Branching-Strategy.png);
