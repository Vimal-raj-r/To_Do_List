# Ex03 To-Do List using JavaScript
## Date:10-03-2025

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM:
## index.html
```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple To-Do</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>To-Do List</h2>
    <input type="text" id="task" placeholder="Enter task...">
    <button onclick="addTask()">Add Task</button>
    
    <ul id="list"></ul>

    <script src="script.js"></script>
</body>
</html>
```
## style.css
```css
body {
    font-family: Arial, sans-serif;
    padding: 20px;
}

input, button {
    padding: 8px;
    margin-bottom: 15px;
}

li {
    margin-bottom: 10px;
    background: #f4f4f4;
    padding: 8px;
    width: 250px;
}

.del-btn {
    color: white;
    background: red;
    border: none;
    padding: 5px;
    margin-left: 15px;
    cursor: pointer;
}
```
## script.js
```js
function addTask() {
    let taskValue = document.getElementById("task").value;
    if (taskValue === "") {
        alert("Enter a task!");
        return;
    }
    let li = document.createElement("li");
    li.innerHTML = taskValue + ' <button class="del-btn" onclick="this.parentElement.remove()">X</button>';
    document.getElementById("list").appendChild(li);
    document.getElementById("task").value = "";
}
```



## OUTPUT:
<img width="1919" height="996" alt="image" src="https://github.com/user-attachments/assets/4ec61509-a794-490c-9c94-946af5770464" />
<img width="1912" height="1000" alt="image" src="https://github.com/user-attachments/assets/63d80c4e-4e32-47b7-b314-2f258946464b" />
<img width="1914" height="992" alt="image" src="https://github.com/user-attachments/assets/4627deb8-813b-469a-98a0-77c8f83d0369" />





## RESULT
The program for creating To-do list using JavaScript is executed successfully.
