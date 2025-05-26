<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>To-Do List - README</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 2rem;
      line-height: 1.6;
    }
    h1, h2, h3 {
      color: #2c3e50;
    }
    ul {
      padding-left: 20px;
    }
    code {
      background: #f4f4f4;
      padding: 2px 6px;
      border-radius: 4px;
    }
    .link {
      color: #2980b9;
      text-decoration: none;
    }
    .link:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <h1>📝 To-Do List React App</h1>

  <p>
    Live Demo: <a class="link" href="https://todolistcelebalcsi.netlify.app" target="_blank">https://todolistcelebalcsi.netlify.app</a>
  </p>

  <h2>📄 Overview</h2>
  <p>
    This React-based To-Do List application allows users to:
  </p>
  <ul>
    <li>Add, remove, and mark tasks as completed</li>
    <li>Sort and filter tasks</li>
    <li>Persist data using <code>localStorage</code></li>
  </ul>

  <h2>🛠️ Prerequisites</h2>
  <ul>
    <li>Node.js and npm installed</li>
    <li>To-Do List React app set up and running locally</li>
  </ul>

  <h2>✅ Test Scenarios</h2>

  <h3>1. Adding a Task</h3>
  <ul>
    <li>Open the app</li>
    <li>Enter a new task</li>
    <li>Click <code>Add Task</code></li>
  </ul>
  <strong>Expected:</strong> Task is added and input field is cleared.

  <h3>2. Removing a Task</h3>
  <ul>
    <li>Add a task (if needed)</li>
    <li>Click <code>Remove</code> button</li>
  </ul>
  <strong>Expected:</strong> Task is removed from the list.

  <h3>3. Marking a Task as Completed</h3>
  <ul>
    <li>Click on task text to toggle completion</li>
  </ul>
  <strong>Expected:</strong> Line-through appears; clicking again unmarks it.

  <h3>4. Filtering Tasks</h3>
  <ul>
    <li>Add multiple tasks, mark some as completed</li>
    <li>Use the filter dropdown</li>
  </ul>
  <strong>Expected:</strong>
  <ul>
    <li><code>All</code>: all tasks</li>
    <li><code>Completed</code>: only completed tasks</li>
    <li><code>Incomplete</code>: only incomplete tasks</li>
  </ul>

  <h3>5. Sorting Tasks</h3>
  <ul>
    <li>Add tasks with different names/statuses</li>
    <li>Use the sort dropdown: Task Name, Creation Date, Completion Status</li>
  </ul>
  <strong>Expected:</strong> Tasks should reorder accordingly.

  <h3>6. Data Persistence</h3>
  <ul>
    <li>Add tasks</li>
    <li>Refresh the page</li>
  </ul>
  <strong>Expected:</strong> Tasks persist using <code>localStorage</code>.

  <h2>🧪 Manual Testing Tips</h2>
  <ul>
    <li>Check for empty task validation</li>
    <li>Test across devices and browsers</li>
    <li>Try duplicate task names</li>
  </ul>

  <h2>🧷 Automated Testing (Optional)</h2>
  <p>
    Use <strong>Jest</strong> and <strong>React Testing Library</strong> to:
  </p>
  <ul>
    <li>Test rendering of the initial component</li>
    <li>Simulate user actions like add/remove/complete</li>
    <li>Validate <code>localStorage</code> behavior</li>
  </ul>

  <h2>🚀 Deployment</h2>
  <p>
    The project is deployed on <strong>Netlify</strong>: <br />
    <a class="link" href="https://todolistcelebalcsi.netlify.app" target="_blank">https://todolistcelebalcsi.netlify.app</a>
  </p>
  <p>
    To deploy your own version:
  </p>
  <ul>
    <li>Build the app using <code>npm run build</code></li>
    <li>Drag the <code>build</code> folder to Netlify or connect the GitHub repo</li>
  </ul>

  <h2>📌 Conclusion</h2>
  <p>
    Use this guide to test and verify that all features are working as intended. Report any bugs or suggest improvements via GitHub issues.
  </p>

</body>
</html>
