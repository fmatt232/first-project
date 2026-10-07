# Daily Tasks

A beginner-friendly to-do list built with HTML, CSS, and JavaScript. No dependencies or build tools required.

## Features

- Add tasks (up to 200 characters).
- Mark tasks complete or incomplete.
- Delete tasks and see how many remain.
- Keep tasks in browser local storage across reloads when available.
- Responsive layout with labeled controls and visible keyboard focus.

## Run locally

1. Download this repository using **Code → Download ZIP**.
2. Extract the ZIP.
3. Open `index.html` in your browser.

Alternatively, clone the repository:

```bash
git clone https://github.com/fmatt232/first-project.git
cd first-project
```

Then open `index.html`. For a consistent local origin, you can serve the folder with Python:

```bash
python -m http.server 8000
```

Visit http://localhost:8000.

## How it works

`index.html` contains the page structure, styling, and JavaScript. Tasks are stored under the `daily-tasks-v1` local storage key. Task text is rendered with `textContent` so it is treated as plain text.

Data stays in the current browser and does not sync between devices. Clearing browser data removes saved tasks. If storage is blocked, the app displays a warning and continues working for the current session.

## Try it out

1. Add two tasks.
2. Complete one and check that the remaining count changes.
3. Reload and check that your tasks are preserved when storage is available.
4. Delete a task.
5. Try keyboard navigation and a narrow window.

## Practice ideas

- Add due dates or categories.
- Add filters for active and completed tasks.
- Split the CSS and JavaScript into separate files.
