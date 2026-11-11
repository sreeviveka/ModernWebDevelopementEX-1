# Exp 1 – React Lab Exercise: Understanding React File Structure

## NAME: V.S.SREE VIVEKA  
## REG NO: 2305001031  

## Aim
To create a basic React application using Vite and understand the purpose of important files and folders in the React project structure.

## Objectives
- Create a React project using Vite.
- Identify important React files and folders.
- Understand the role of `main.jsx`, `App.jsx`, `index.html`, and `package.json`.
- Create and use simple React components.
- Run and test a React application.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest student-app
cd student-app
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: Understand the File Structure

```text
student-app/
│
├── node_modules/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── Student.jsx
│   │   ├── Course.jsx
│   │   └── Faculty.jsx
│   │
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── index.html
├── package.json
├── package-lock.json
└── vite.config.js
```

### Step 3: Understand index.html

The `index.html` file contains the root element where the React application is displayed.

```html
<div id="root"></div>
```

### Step 4: Understand main.jsx

The `main.jsx` file is the entry point of the React application. It connects React with the HTML root element and renders the App component.

### Step 5: Create App.jsx

```jsx
import './App.css'

function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>

      <Student />
      <Course />
      <Faculty />
    </div>
  )
}

export default App
```

### Step 6: Create Student.jsx

Create a `components` folder inside `src` and add `Student.jsx`.

```jsx
import '../App.css'

function Student() {
  return (
    <div className="student">
      <h2>Student Details</h2>

      <p>Name: SREE VIVEKA</p>
      <p>Register Number: 2305001031</p>
      <p>Department: CSE</p>
    </div>
  )
}

export default Student
```

### Step 7: Create Course.jsx

```jsx
import '../App.css'

function Course() {
  return (
    <div className="student">
      <h2>Course Details</h2>

      <p>Course: AI1067 - WEB DEVELOPEMENT</p>
      <p>Semester: 7</p>
      <p>Credits: 3</p>
    </div>
  )
}

export default Course
```

### Step 8: Create Faculty.jsx

```jsx
import '../App.css'

function Faculty() {
  return (
    <div className="student">
      <h2>Faculty Details</h2>

      <p>Name: Ajith Kumar</p>
      <p>Department: CSE</p>
      <p>Designation: Professor</p>
      
    </div>
  )
}

export default Faculty
```

### Step 9: Import Components in App.jsx

```jsx

import './App.css'
import Student from './components/Student'
import Course from './components/Course'
import Faculty from './components/Faculty'

function App() {
  return (
    <div className="container">
      <h1>Student Information System</h1>

      <Student />
      <Course />
      <Faculty />
    </div>
  )
}

export default App

```

### Step 10: Add CSS in App.css

```css
.container {
  text-align: center;
  padding: 30px;
}

.student {
  border: 1px solid #ccc;
  padding: 20px;
  margin: 20px auto;
  width: 300px;
}

.student h2 {
  color: blue;
}

.student p {
  color: green;
}
```

## Output

### Student Information System

<img width="828" height="777" alt="WhatsApp Image 2026-11-11 at 9 30 07 AM" src="https://github.com/user-attachments/assets/362d2ce6-3af4-48ce-8b4a-f364a05177da" />

## Result

Thus, a basic React application was successfully created using Vite. The React file structure was understood, and reusable components were created and displayed successfully.
