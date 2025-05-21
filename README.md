import React from 'react';
import ReactDOM from 'react-dom/client';

// This is our simple App component that displays "Hello World!"
function App() {
  return (
    <main>
      <h1>Hello World!</h1>
    </main>
  );
}

// Find the root element in the HTML
const container = document.getElementById('root');

// Create a root using React 18's createRoot API
const root = ReactDOM.createRoot(container);

// Render the App component wrapped in React.StrictMode for highlighting potential problems
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
