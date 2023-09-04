# Husky Demo App

Welcome to the Husky Demo App repository! This project is built using Vite with the React TypeScript template and includes configuration for pre-commit hooks using Husky.

## Overview

This demo app is a minimalistic React application scaffolded with Vite, a fast development build tool. It showcases the integration of Husky for pre-commit hooks to automate tasks like linting and formatting before committing your code.

## Usage

### Prerequisites

Before you begin, make sure you have the following installed on your system:

- Node.js (v14 or higher)
- npm (Node Package Manager)

### Getting Started

1. Clone the Repository:

   ```bash
   git clone https://github.com/ManishPJha/husky-demo-app.git
   cd husky-demo-app
   ```

2. Install Dependencies:

   ```bash
   npm install
   ```

### Available Scripts

You can run the following npm scripts:

- `npm run dev`: Start the development server with Vite.
- `npm run build`: Build the project for production.
- `npm run format`: Format code using Prettier.
- `npm run lint`: Lint your TypeScript and React code using ESLint.
- `npm run preview`: Preview the production build locally.

### Pre-commit Hooks

This project uses Husky and lint-staged to enforce code quality checks before committing. When you run `git commit`, Husky will automatically run the configured tasks for you.

The pre-commit configuration is defined in the `.husky/pre-commit` file. Here's what it does:

```shell
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"

npx lint-staged
```

It runs `lint-staged`, which in turn runs ESLint and Prettier on the files that are about to be committed.

### Dependencies

- `@reduxjs/toolkit`: A library for Redux state management.
- `prettier`: A code formatter to keep your code consistent.
- `react`, `react-dom`: Core React libraries.
- `react-redux`: Official React bindings for Redux.
- `react-router-dom`: React Router for navigation.

### Dev Dependencies

- `@types/react`, `@types/react-dom`: TypeScript type definitions for React.
- `@typescript-eslint/eslint-plugin`, `@typescript-eslint/parser`: ESLint plugins for TypeScript.
- `@vitejs/plugin-react`: Vite plugin for React.
- `eslint`: ESLint for code linting.
- `eslint-plugin-react-hooks`, `eslint-plugin-react-refresh`: ESLint plugins for React best practices.
- `husky`: Git hooks made easy.
- `lint-staged`: Run linters on pre-committed files.
- `typescript`: TypeScript language support.
- `vite`: Build tool for frontend development.

## License

This project is licensed under the MIT License. Feel free to use it, modify it, and distribute it as needed for your projects. Please refer to the [LICENSE](LICENSE) file for more information.

## Contributions

Contributions are welcome! If you have suggestions, bug reports, or want to contribute to this project, please open an issue or create a pull request.

Happy coding with Husky Demo App! 🚀
