
<p align="center">
  <a href="https://www.chromatic.com/">
    <img alt="Chromatic" src="https://avatars2.githubusercontent.com/u/24584319?s=200&v=4" width="60" />
  </a>
</p>

<h1 align="center">
  Chromatic's Intro to Storybook React template
</h1>

This template ships with the main React and Storybook configuration files you'll need to get up and running fast.

## 🚅  Quick start

1.  **Create the application.**

    Use [degit](https://github.com/Rich-Harris/degit) to get this template.

    ```shell
    # Clone the template
    npx degit chromaui/intro-storybook-react-template taskbox
    ```

1.  **Install the dependencies.**

    Navigate into your new site’s directory and install the necessary dependencies.

    ```shell
    # Navigate to the directory
    cd taskbox/

    # Install the dependencies
    yarn
    ```

1.  **Open the source code and start editing!**

    Open the `taskbox` directory in your code editor of choice and building your first component!

1.  **Browse your stories!**

    Run `yarn storybook` to see your component's stories at `http://localhost:6006`

## 🔎 What's inside?

A quick look at the top-level files and directories included with this template.

    .
    ├── .storybook
    ├── node_modules
    ├── public
    ├── src
    ├── .env
    ├── .gitignore
    ├── LICENSE
    ├── package.json
    ├── yarn.lock
    └── README.md


1.  **`.storybook`**: This directory contains Storybook's [configuration](https://storybook.js.org/docs/react/configure/overview) files.

2.  **`node_modules`**: This directory contains all of the modules of code that your project depends on (npm packages).

3.  **`public`**: This directory will contain the development and production build of the site.

4.  **`src`**: This directory will contain all of the code related to what you will see on your application.

5.  **`.env`**: Simple text configuration file for controlling the application's environment constants.

6.  **`.gitignore`**: This file tells git which files it should not track or maintain during the development process of your project.

7. **`LICENSE`**: The template is licensed under the MIT licence.

8. **`package.json`**: Standard manifest file for Node.js projects, which typically includes project specific metadata (such as the project's name, the author among other information). It's based on this file that npm will know which packages are necessary to the project.

9. **`yarn.lock`**: This is an automatically generated file based on the exact versions of your npm dependencies that were installed for your project. **(Do not change it manually).**

10. **`README.md`**: A text file containing useful reference information about the project.

## Contribute

If you encounter an issue with the template, we encourage you to open an issue in this template's repository.

## Learning Storybook

1. Read our introductory tutorial at [Learn Storybook](https://storybook.js.org/tutorials/intro-to-storybook/react/en/get-started/).
2. Learn how to transform your component libraries into design systems in our [Design Systems for Developers](https://storybook.js.org/tutorials/design-systems-for-developers/) tutorial.
2. See our official documentation at [Storybook](https://storybook.js.org/).


### FAQ

## What is Component-Driven Development
Component-Driven Development allows you to gradually expand complexity as you move up the component hierarchy. Among the benefits are a more focused development process and increased coverage of all possible UI permutations. In short, CDD helps you build higher-quality and more complex user interfaces.

## What is a story defined?
To define our stories, we export a function for each of our test states to generate a story. The story is a function that returns a rendered element (i.e. a component with a set of props) in a given state---exactly like a Functional Component.

## Convenient variable 'Template'
We use Template to reduce the amount of code written. Template.
`Template.bind({}) is a standard JavaScript technique for making a copy of a function. We use this technique to allow each exported story to set its own properties, but use the same implementation.`

## What are actions
 Actions help you verify interactions when building UI components in isolation. Oftentimes you won't have access to the functions and state you have in context of the app. Use action() to stub them in.
## What do actions do?
actions allows us to create callbacks that appear in the actions panel of the Storybook UI when clicked. So when we build a pin button, we’ll be able to determine in the test UI if a button click is successful.

## What are parameters?
parameters are typically used to control the behavior of Storybook's features and addons. In our case we're going to use them to configure how the actions (mocked callbacks) are handled.


## Tutorial 2 - Building a Design system for production

## What is a Design System?
Design systems contain reusable UI components that help teams build complex, durable, and accessible user interfaces across projects. Since both designers and developers contribute to the UI components, the design system serves as a bridge between disciplines. It is also the “source of truth” for an organization’s common components.

There are three technical parts to a design system that we’ll talk about in this guide:

* 🏗 Common reusable UI components
* 🎨 Design tokens: Styling-specific variables such as brand colors and spacing
* 📕 Documentation site: Usage instructions, narrative, do’s and don'ts

## Components for a design system:
# Build components
* 📚 Storybook for UI component development and auto-generated docs
⚛️ React for declarative component-centric UI (via create-react-app)
* 💅 Styled-components for component-scoped styling
* ✨ Prettier for automatic code formatting
# Maintain the system
* 🚥 GitHub Actions for continuous integration
* 📐 ESLint for JavaScript linting
* ✅ Chromatic to catch visual bugs in components (by Storybook maintainers)
* 🃏 Jest for unit testing components
* 📦 npm for distributing the library
* 🛠 Auto for release management workflow
# Storybook addons
* ♿ Accessibility to check for accessibility issues during development
* 💥 Actions to QA click and tap interactions
* 🎛 Controls to interactively adjust props to experiment with components
* 📕 Docs for automatic documentation generation from stories

Reference to Storybook's Design system: https://github.com/storybookjs/design-system