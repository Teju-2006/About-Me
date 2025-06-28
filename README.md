# About-Me
# 👋 Hi, I'm Teja Lakshmi Chappa!

Welcome to my GitHub profile! Here’s a quick overview of who I am and what I do:

## 🚀 About Me

- 👩‍🎓 **Status:** Student
- 🌱 **Learning:** Python, HTML, CSS, JavaScript
- ❓ **Currently Exploring:** Still figuring out some areas—open to learning and discovering new things!
- 🤝 **Open to Collaboration:** Yes! I'm eager to work on projects and learn from others.
- 📦 **Projects:** See below for what I'm working on!

## 🛠️ Skills

- **Languages:** Python, HTML, CSS, JavaScript

## 💡 Projects

### 📝 [Task Manager](#task-manager-code)
A simple Task Manager web app built using **HTML, CSS, and JavaScript**.  
This project helps in organizing daily tasks effectively and is a great example of front-end development skills.

---

<details>
<summary id="task-manager-code">📂 <b>Task Manager Code</b> (Click to expand)</summary>

#### `index.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Task Manager</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>Task Manager</h1>
    <input type="text" id="taskInput" placeholder="Add a new task..." />
    <button onclick="addTask()">Add Task</button>
    <ul id="taskList"></ul>
  </div>
  <script src="script.js"></script>
</body>
</html>
```

#### `style.css`
```css
body {
  font-family: Arial, sans-serif;
  background: #f4f4f4;
}
.container {
  max-width: 400px;
  margin: 40px auto;
  background: #fff;
  padding: 24px;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
h1 {
  text-align: center;
  color: #333;
}
input[type="text"] {
  width: 70%;
  padding: 8px;
  margin-right: 5px;
  border-radius: 4px;
  border: 1px solid #ccc;
}
button {
  padding: 8px 12px;
  background: #007bff;
  color: #fff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
button:hover {
  background: #0056b3;
}
ul#taskList {
  list-style: none;
  padding: 0;
  margin-top: 16px;
}
ul#taskList li {
  padding: 8px 0;
  border-bottom: 1px solid #eee;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
ul#taskList li.completed {
  text-decoration: line-through;
  color: #888;
}
.delete-btn {
  background: #dc3545;
  color: #fff;
  border: none;
  padding: 4px 8px;
  border-radius: 4px;
  cursor: pointer;
}
.delete-btn:hover {
  background: #a71d2a;
}
```

#### `script.js`
```javascript
const taskInput = document.getElementById('taskInput');
const taskList = document.getElementById('taskList');

function addTask() {
  const taskText = taskInput.value.trim();
  if (taskText === "") return;

  const li = document.createElement('li');
  li.textContent = taskText;

  li.addEventListener('click', () => {
    li.classList.toggle('completed');
  });

  const delBtn = document.createElement('button');
  delBtn.textContent = "Delete";
  delBtn.className = "delete-btn";
  delBtn.onclick = (e) => {
    e.stopPropagation();
    li.remove();
  };

  li.appendChild(delBtn);
  taskList.appendChild(li);
  taskInput.value = "";
}
```
</details>

---

## 📚 Goals

- Start contributing to open source projects
- Build and showcase my own projects
- Keep learning and growing as a developer

## 📫 Connect with Me

- [LinkedIn](https://www.linkedin.com/in/teja-lakshmi-chappa)
- [Email](mailto:tejalakshmichappa@gmail.com)
- 📞 Contact No: +91-8897101097

---

Thanks for stopping by! 🚀
