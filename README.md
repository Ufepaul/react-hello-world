Full Code for Hello World React App
This setup follows React 18 best practices, using functional components and semantic HTML.

1. public/index.html (HTML structure)
This is the basic HTML file where your React app will be mounted.
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hello World React App</title>
  </head>
  <body>
    <div id="root"></div> <!-- React app will be mounted here -->
  </body>
</html>



2. src/App.js (React Component)
This is your main React component, displaying "Hello World!".
import React from 'react';

function App() {
  return (
    <main>
      <h1>Hello World!</h1>
    </main>
  );
}

export default App;



3. src/index.js (Entry point)
This file initializes the React app using React 18's createRoot API.
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';

const container = document.getElementById('root');
const root = ReactDOM.createRoot(container);

root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);



Running the App
- Install Node.js if you haven't already.
- Create the React project:
npx create-react-app hello-world
- Navigate into the project folder:
cd hello-world
- Replace the contents of public/index.html, src/App.js, and src/index.js with the above code.
- Start the development server:
npm start

Your browser should open http://localhost:3000, displaying "Hello World!" 


