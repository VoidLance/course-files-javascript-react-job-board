# React Job Board

A small React job-board dashboard for **Scopt Enterprises**. The app displays the
number of jobs scheduled today and an estimate for next week, with messages that
change for quiet, normal, and busy days.

## Why use this project?

- Provides a focused example of composing a React application from components.
- Demonstrates JSX expressions, conditional rendering, template literals, and
  inline styles.
- Uses Create React App for a familiar development server, test runner, and
  production build.
- Includes a responsive, dark dashboard presentation with separate styling for
  today's and next week's job summaries.

The current dashboard uses sample values in [`src/JobBoard.js`](src/JobBoard.js).
It is intended as a lightweight starting point for connecting a real jobs API,
adding filters, or expanding the board into a larger scheduling workflow.

## Getting started

### Prerequisites

- Node.js and npm
- A modern web browser

### Install

Clone the repository, enter the project directory, and install its dependencies:

```bash
git clone https://github.com/VoidLance/course-files-javascript-react-job-board.git
cd course-files-javascript-react-job-board
npm install
```

### Run the development server

```bash
npm start
```

Open <http://localhost:3000> in your browser. The page reloads automatically
when source files change.

### Use the dashboard

The displayed company, job count, and estimate are configured near the top of
[`JobBoard`](src/JobBoard.js):

```js
const companyName = "Scopt Enterprises";
const jobCount = 5;
const nextWeekJobs = jobCount * 1.5;
```

Change `jobCount` and save the file to see the dashboard message switch between
no jobs, a normal day, and a busy day.

## Available commands

| Command | Purpose |
| --- | --- |
| `npm start` | Start the local development server. |
| `npm test` | Run the Jest and React Testing Library test suite. |
| `npm run build` | Create an optimized production bundle in `build/`. |
| `npm run eject` | Copy Create React App configuration into the project. This is irreversible and usually unnecessary. |

## Project structure

```text
public/              Static HTML, manifest, icons, and robots.txt
src/App.js           Application shell
src/JobBoard.js      Job summary component and sample dashboard logic
src/App.css          Dashboard layout and component styles
src/index.js         React entry point
src/App.test.js      Application tests
package.json         Scripts and dependencies
```

## Help and documentation

For project questions or bug reports, [open an issue on
GitHub](https://github.com/VoidLance/course-files-javascript-react-job-board/issues).
For framework and tooling reference, see the [React
documentation](https://react.dev/) and [Create React App
documentation](https://create-react-app.dev/docs/getting-started/).

## Contributing

Contributions are welcome:

1. Fork the repository and create a focused feature or fix branch.
2. Install dependencies with `npm install`.
3. Make and test your changes with `npm test` and, when relevant,
   `npm run build`.
4. Open a pull request with a clear summary of the change and its verification.

Please keep changes focused and update relevant tests when behavior changes.

## Maintainer

This project is maintained by [VoidLance](https://github.com/VoidLance).
