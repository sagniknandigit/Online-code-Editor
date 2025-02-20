# Online Code Editor

This project is an online code editor built using [CodeMirror](https://codemirror.net/), a versatile text editor implemented in JavaScript for the browser. The editor supports syntax highlighting for various languages, real-time editing, and more.

## Features

- Syntax highlighting for popular programming languages
- Real-time editing
- Customizable themes
- Line numbering and code indentation
- Language mode support (e.g., JavaScript, Python, HTML, CSS)
- Keyboard shortcuts for common code editor commands

## Prerequisites

Before running this project, ensure that you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (version 12.x or above)
- [npm](https://www.npmjs.com/) (Node package manager)

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/online-code-editor.git
   ```

2. Navigate to the project directory:

   ```bash
   cd online-code-editor
   ```
3. To fix the node dependencies using npm:

   ```bash
   npm audit fix
   npm install --force

4. To generate the package.json
   ```bash
   npm init
   ```
   press enter until the new command line appears

4. Install the required dependencies using npm:

   ```bash
   npm install express body-parser compilex nodemon
   ```

5. Start the development server:

   ```bash
   nodemon Api.js
   ```

   The application will be available at `http://localhost:3000`.

## Usage

1. **Code Editing**: The editor supports multiple languages. You can switch between different programming languages by selecting the appropriate mode (e.g., JavaScript, Python, HTML).
   
2. **Themes**: Customize the editor’s appearance by changing the theme. Several themes (e.g., `monokai`, `material`, `dracula`) are included by default.

3. **Shortcuts**: You can use keyboard shortcuts like:

   - `Ctrl + S` to save code
   - `Ctrl + /` to comment/uncomment a line
   - `Ctrl + Z` to undo
   
4. **Customization**: Modify the editor's configuration by editing the `src/config/codemirror.js` file.

## CodeMirror Configuration

The CodeMirror editor is configured in the `src/config/codemirror.js` file. You can customize:

- **Mode**: Define the language mode (e.g., JavaScript, Python).
- **Theme**: Choose from a variety of available themes.
- **Line Numbers**: Enable or disable line numbering.
- **Tab Size**: Adjust the size of indentation.

Example configuration:

```javascript
import CodeMirror from 'codemirror';
import 'codemirror/mode/javascript/javascript';
import 'codemirror/theme/monokai.css';

const editorConfig = {
  lineNumbers: true,
  mode: 'javascript',
  theme: 'monokai',
  tabSize: 2,
};

export default editorConfig;
```

## Available Scripts

In the project directory, you can run:

- **`nodemon Api.js`**: Runs the app in development mode.

## Dependencies

- [CodeMirror](https://codemirror.net/) – Code editor library for syntax highlighting.
- [React](https://reactjs.org/) – JavaScript library for building user interfaces (if applicable).
