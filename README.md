Task List

A small task list built with plain HTML, CSS and JavaScript. No frameworks, no build step.

Live demo: https://coilwer.github.io/task-list/

Features
Add, complete and delete tasks
Filter by All, Active or Done
Clear all completed tasks at once
Tasks are saved in the browser (localStorage), so they stay after a reload
Keyboard friendly: labelled checkboxes, aria-pressed on filter buttons, visible focus states
Responsive layout
Tech
HTML5
CSS3 (custom properties, flexbox)
JavaScript (ES6, DOM API, localStorage)
Run locally
bash
git clone https://github.com/coilwer/task-list.git
cd task-list

Then open index.html in a browser. There is nothing to install.

How it works
State is one array of { id, text, done } objects.
Every change updates the array, saves it to localStorage and redraws the list with render().
User input is inserted with textContent, so it is never parsed as HTML.
Storage calls are wrapped in try/catch, so the app still works if the browser blocks localStorage.
What I practised
Working with the DOM and events without a framework
Keeping UI in sync with state
Basic accessibility and safe handling of user input
Author

Oleksandr Plotnikov, GitHub
