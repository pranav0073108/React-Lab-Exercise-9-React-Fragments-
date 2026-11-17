# React-Lab-Exercise-9-React-Fragments-
## Name : PRANAV K
## Register Number : 2305001026

# Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary DOM elements.

# Program:
## App.jsx
```python
import { Fragment } from "react";
import "./App.css";

function Student() {
  return (
    <>
      <h2>Student Details</h2>
      <p>Name: Ajith</p>
      <p>Department: CSE</p>
      <p>Year: III Year</p>
    </>
  );
}

function App() {
  const students = [
    { id: 1, name: "Ajith" },
    { id: 2, name: "Ravi" },
    { id: 3, name: "Divya" },
  ];

  return (
    <div className="container">
      <h1>College Information</h1>
      <Student />
      <hr />
      <h2>Student List</h2>
      {students.map((student) => (
        <Fragment key={student.id}>
          <h3>{student.name}</h3>
          <p>Department: Computer Science</p>
          <hr />
        </Fragment>
      ))}
    </div>
  );
}

export default App;

```

# Output:

<img width="900" height="435" alt="image" src="https://github.com/user-attachments/assets/3c6362fd-d1f7-4524-8e21-9ff67e9db3d2" />

<img width="901" height="436" alt="image" src="https://github.com/user-attachments/assets/260c937b-0828-407c-991a-096fbf7d6f32" />

# Result:
Thus, React Fragments were successfully implemented using both shorthand syntax (<> </>) 
and explicit Fragment syntax. Multiple JSX elements were grouped without adding extra 
wrapper elements to the DOM. 




