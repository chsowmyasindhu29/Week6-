import React from 'react';
import './App.css';

function App() {
                const [count, setCount] = useState(0);

  const student = {
    name: 'Ravi',
    branch: 'CSE',
    year: 'II B.Tech'
  };

  return (
    <div className="container">
     <h1>Props and State Demo</h1>

      <Student name="Ravi" />

      <h3>Count: {count}</h3>

      <button onClick={() => setCount(count + 1)}>
        Increase
      </button>

      <h1>Student Details</h1>

      <div className="card">
        <h2>{student.name}</h2>
        <p>Branch: {student.branch}</p>
        <p>Year: {student.year}</p>
      </div>
    </div>
  );
}

export default App;
App.css
    
.container {
  text-align: center;
  font-family: Arial, sans-serif;
  margin-top: 40px;
}

.container h1 {
  color: navy;
}

.card {
  background-color: #e6f2ff;
  border: 2px solid navy;
  border-radius: 10px;
  padding: 20px;
  margin: 20px auto;
  width: 250px;
}

.card h2 {
  color: darkgreen;
}
