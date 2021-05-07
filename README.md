<h1 align="center">
   🕆 <a href="https://github.com/filipeveronezi/ibt-web/"> IBT WEB </a>
</h1>

<h3 align="center">
  <a href="https://ibt.filipeveronezi.dev.br/">ibt.filipeveronezi.dev.br</a>
</h3>

<h4 align="center"> 
	 Status: In progress
</h4>

<p align="center">
 <a href="#layout">Layout</a> •
 <a href="#tech-stack">Tech Stack</a> • 
 <a href="https://github.com/filipeveronezi">Author</a>
</p>

---

## Layout

The application layout is available on Figma:

<a href="https://www.figma.com/file/uUMjHET1lVbnIsHDSF8vDZ/IBT-WEB?node-id=0%3A1">
  <img alt="Layout" src="https://img.shields.io/badge/Layout%20-Figma-%2304D361">
</a>

---

## Pre-requisites

Before you begin, you will need to have the following tools installed on your machine:
- [Git] (https://git-scm.com)
- [Node.js] (https://nodejs.org/en/)
- Editor to work with the code like [VSCode] (https://code.visualstudio.com/)
- (optional) [Yarn] (https://yarnpkg.com/)

---

## Running the web application for development

```bash

# Clone this repository
$ git clone git@github.com:filipeveronezi/ibt-web.git

# Access the project folder in your terminal
$ cd ibt-web

# Install the dependencies
$ npm install

# Run the application in development mode
$ npm run dev

# The application will open on the port 3000 of your local host

```

You can also run the application with:

```bash

$ npm run dev:shared

```

This will allow access for the application on the port 8080, including external devices through your machine's IP address. This is useful for testing the mobile layout.

---

## Tech Stack

The following tools are being used in the construction of the project:

-   **[Nuxt.js](https://nuxtjs.org/)**
-   **[Typescript](https://www.typescriptlang.org/)**
-   **[Vue.js](https://vuejs.org/)**
-   **[Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/)**
-   **[Vuex](https://vuex.vuejs.org/)**
-   **[Vuex Module Decorators](https://github.com/championswimmer/vuex-module-decorators)**
-   **[Axios](https://axios.nuxtjs.org/)**
-   **[Normalize.css](https://necolas.github.io/normalize.css/)**

### Linting tools

-   **[ESLint](https://eslint.org/)**
-   **[Prettier](https://prettier.io/)**

### **Other**

-   Editor:  **[Visual Studio Code](https://code.visualstudio.com/)**
-   Deploy on:  **[GitHub Pages](https://pages.github.com/)**
