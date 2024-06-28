# Sudoku

Multiplayer Sudoku game through node, express, tailwind, socket.

## Prerequisites

- Node.js (version 14 or higher)
- npm (version 6 or higher)

## Setup

1. **Clone the repository**:

    ```bash
    git clone https://github.com/starryxvii/sudoku.git
    cd sudoku
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Configure Tailwind CSS**:

    Tailwind CSS and its plugins are already configured in this project. The configuration files are:

    - `tailwind.config.js`: Configures Tailwind CSS.
    - `postcss.config.js`: Configures PostCSS to use Tailwind CSS and Autoprefixer.

4. **Start the development server**:

    ```bash
    npm run dev
    ```

    This command uses `concurrently` to run both `webpack` in watch mode and `nodemon` to restart the server upon changes.

## Commands

### `npm run build`

- **Purpose**: Builds the project for production by running Webpack, which compiles the source files from the `src` directory and outputs them to the `public` directory.
- **Usage**: Run this command whenever you want to create a production build of your project.

    ```bash
    npm run build
    ```

### `npm start`

- **Purpose**: Starts the Express server to serve the files from the `public` directory.
- **Usage**: Run this command to start the server after building the project.

    ```bash
    npm start
    ```

### `npm run dev`

- **Purpose**: Runs the development server with live reloading and recompilation. It uses `concurrently` to run both `webpack --watch` to recompile assets on changes and `nodemon` to restart the server on changes to server files.
- **Usage**: Run this command during development to automatically recompile assets and restart the server on file changes.

    ```bash
    npm run dev
    ```