# CodePen Clone

A simple and interactive CodePen Clone built with React that allows users to write HTML, CSS, and JavaScript code and instantly preview the output in real time. This project was created to practice React concepts, state management, and code editor integration.

---

## 🚀 Features

- Live HTML Editor
- Live CSS Editor
- Live JavaScript Editor
- Real-Time Output Preview
- Responsive User Interface
- Separate Editors for HTML, CSS, and JavaScript
- Instant Code Compilation and Rendering
- Syntax Highlighting

---

## 🛠️ Technologies Used

- React.js
- HTML5
- CSS3
- JavaScript (ES6+)

---

## 📚 Libraries Used

### CodeMirror

```json
"codemirror": "^5.57.0"
```

CodeMirror is used to provide a professional code editing experience inside the browser. It offers:

- Syntax Highlighting
- Line Numbers
- Code Formatting Support
- Better Code Readability
- Improved User Experience

### React CodeMirror

```json
"react-codemirror2": "^7.2.1"
```

React CodeMirror is a React wrapper around CodeMirror. It makes it easy to integrate the CodeMirror editor into React applications and manage editor state using React components.

### React

```json
"react": "^16.13.1"
"react-dom": "^16.13.1"
```

React is used to build the user interface and manage application state efficiently.

---

## ⚠️ Why Older CodeMirror Libraries Were Used

Initially, newer CodeMirror versions were tested in this project. However, they introduced several compatibility issues, including:

- Incorrect text rendering inside the editor.
- Characters appearing in reverse order while typing.
- Output synchronization issues.
- Additional integration problems with the project setup.

For example, typing:

```text
hello
```

sometimes produced unexpected editor behavior and rendering issues.

To ensure stability and compatibility, the project uses the older and well-supported versions:

```json
"codemirror": "^5.57.0"
"react-codemirror2": "^7.2.1"
```

These versions provided a more reliable development experience and worked correctly with the project's React version.

---

## 📦 Installation

Clone the repository:

```bash
git https://github.com/abrar0349/code-pen-clone.git
```

Navigate to the project folder:

```bash
cd codepen-clone
```

Install dependencies:

```bash
npm install
```

---

## ▶️ Running the Project

The project uses the following start script:

```json
"start": "set NODE_OPTIONS=--openssl-legacy-provider && react-scripts start"
```

Run the project using:

```bash
npm start
```

---

## 🔧 Why Is `--openssl-legacy-provider` Used?

Modern versions of Node.js use OpenSSL 3 by default. Older React projects created with Create React App and some older dependencies may not be fully compatible with OpenSSL 3.

Without this configuration, the application may fail to start and display errors similar to:

```bash
error:0308010C:digital envelope routines::unsupported
```

To solve this issue, the following flag is used:

```bash
--openssl-legacy-provider
```

### What Does It Do?

```bash
set NODE_OPTIONS=--openssl-legacy-provider
```

This command:

- Enables legacy OpenSSL support.
- Allows older React dependencies to work with newer Node.js versions.
- Prevents OpenSSL compatibility errors.
- Ensures the development server starts successfully.

The second part:

```bash
react-scripts start
```

starts the React development server and runs the application locally.

---

## 📂 Project Structure

```text
src/
│
├── components/
│   ├── Editor.js
│   ├── Preview.js
│   └── ...
│
├── App.js
├── App.css
└── index.js
```

---

## 🎯 Learning Objectives

This project helped in understanding:

- React Components
- React Hooks
- State Management
- Props
- Third-Party Library Integration
- Live Code Rendering
- CodeMirror Integration
- Real-Time UI Updates

---

## 📸 Preview

The application provides three separate editors:

- HTML Editor
- CSS Editor
- JavaScript Editor

The output panel updates automatically whenever code changes are made.

---

## 🤝 Future Improvements

- Dark/Light Theme Toggle
- Save Code Functionality
- Download Project Files
- User Authentication
- Multiple Templates
- Auto-Save Feature
- Code Formatting Support

---

## 👨‍💻 Author

**Abrar Khan**

Frontend Developer passionate about React.js and modern web development.

### Skills

- HTML5
- CSS3
- JavaScript (ES6+)
- Bootstrap
- Tailwind CSS
- React.js
- Redux
- Next.js
- Express.js
- MongoDB

---

## 📄 License

This project is created for learning and educational purposes.