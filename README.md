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
      background-color: #fdfdfd;
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
      font-family: monospace;
    }
    .link {
      color: #2980b9;
      text-decoration: none;
    }
    .link:hover {
      text-decoration: underline;
    }
    .section {
      margin-bottom: 2rem;
    }
  </style>
</head>
<body>

  <h1>📝 To-Do List Component</h1>

  <div class="section">
    <p><strong>Live Demo:</strong> <a class="link" href="https://todolistcelebalcsi.netlify.app/" target="_blank">https://todolistcelebalcsi.netlify.app/</a></p>
  </div>

  <div class="section">
    <h2>📄 Overview</h2>
    <p>This document provides guidance on how to test the To-Do List component to ensure its functionality and reliability.</p>
    <p>The To-Do List component allows users to:</p>
    <ul>
      <li>Add, remove, and mark tasks as completed</li>
      <li>Sort and filter tasks</li>
      <li>Persist data using <code>localStorage</code></li>
    </ul>
  </div>

  <div class="section">
    <h2>🛠️ Prerequisites</h2>
    <ul>
      <li>Node.js and npm installed</li>
      <li>The To-Do List React app set up and running locally</li>
    </ul>
  </div>

  <div class="section">
    <h2>✅ Test Scenarios</h2>

    <h3>1. Adding a Task</h3>
    <ul>
      <li>Open the To-Do List application.</li>
      <li>Enter a new task in the input field.</li>
      <li>Click the <code>Add Task</code> button.</li>
    </ul>
    <p><strong>Expected Outcome:</strong> The new task should appear in the task list and the input field should be cleared.</p>

    <h3>2. Removing a Task</h3>
    <ul>
      <li>Add a task if none are present.</li>
      <li>Click the <code>Remove</code> button next to the task you want to delete.</li>
    </ul>
    <p><strong>Expected Outcome:</strong> The selected task should be removed from the task list.</p>

    <h3>3. Marking a Task as Completed</h3>
    <ul>
      <li>Add a task if none are present.</li>
      <li>Click on the task text to mark it as completed.</li>
    </ul>
    <p><strong>Expected Outcome:</strong> The task text should have a line-through. Clicking again should unmark it.</p>

    <h3>4. Filtering Tasks</h3>
    <ul>
      <li>Add multiple tasks, marking some as completed.</li>
      <li>Use the filter dropdown to select <code>All</code>, <code>Completed</code>, or <code>Incomplete</code>.</li>
    </ul>
    <p><strong>Expected Outcome:</strong></p>
    <ul>
      <li><code>All</code>: All tasks are displayed</li>
      <li><code>Completed</code>: Only completed tasks are shown</li>
      <li><code>Incomplete</code>: Only incomplete tasks are shown</li>
    </ul>

    <h3>5. Sorting Tasks</h3>
    <ul>
      <li>Add multiple tasks with different names and statuses.</li>
      <li>Use the sort dropdown (e.g., <code>Task Name</code>, <code>Creation Date</code>, <code>Completion Status</code>).</li>
    </ul>
    <p><strong>Expected Outcome:</strong> Tasks should reorder accordingly based on the selected sorting criteria.</p>

    <h3>6. Data Persistence</h3>
    <ul>
      <li>Add multiple tasks.</li>
      <li>Refresh the browser.</li>
    </ul>
    <p><strong>Expected Outcome:</strong> The tasks should persist and appear in the task list after reload using <code>localStorage</code>.</p>
  </div>

  <div class="section">
    <h2>🧪 Manual Testing Tips</h2>
    <ul>
      <li>Ensure that empty tasks cannot be added.</li>
      <li>Verify the app works across different browsers and devices.</li>
      <li>Test edge cases such as adding tasks with duplicate names.</li>
    </ul>
  </div>

  <div class="section">
    <h2>🧷 Automated Testing (Optional)</h2>
    <p>Consider writing automated tests using <code>Jest</code> and <code>React Testing Library</code>.</p>
    <ul>
      <li>Test component rendering and initial state.</li>
      <li>Simulate user actions like adding/removing/completing tasks.</li>
      <li>Verify <code>localStorage</code> behavior is working correctly.</li>
    </ul>
  </div>

  <div class="section">
    <h2>🚀 Deployment</h2>
    <p>The project is deployed on <strong>Netlify</strong>:</p>
    <p><a class="link" href="https://todolistcelebalcsi.netlify.app/" target="_blank">https://todolistcelebalcsi.netlify.app/</a></p>
    <p><strong>To deploy your own version:</strong></p>
    <ul>
      <li>Run <code>npm run build</code></li>
      <li>Deploy the <code>build</code> folder to Netlify</li>
      <li>Or connect your GitHub repo to Netlify directly</li>
    </ul>
  </div>

  <div class="section">
    <h2>📌 Conclusion</h2>
    <p>Use this guide to thoroughly test and ensure all features of your To-Do List component function correctly. Log bugs and improvements through GitHub Issues or any issue tracking system you're using.</p>
  </div>

</body>
</html>
