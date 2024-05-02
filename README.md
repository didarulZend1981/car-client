# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

  ###cmd/mode.jsx
      npm create vite@latest name-of-your-project -- --template react
      npm install react-router-dom localforage match-sorter sort-by
      npm install -D tailwindcss postcss autoprefixer
      npx tailwindcss init -p
      tailwind.config.js
      @tailwind base;
      @tailwind components;
      @tailwind utilities;
  ### src/main.jsx
      
      import ReactDOM from 'react-dom/client'
      import './index.css'
      import {
 
        RouterProvider,
      } from "react-router-dom";
      import router from './Routes/Routes.jsx';

      ReactDOM.createRoot(document.getElementById('root')).render(
         <React.StrictMode>
            <RouterProvider router={router} />
         </React.StrictMode>,
       )
  
  ### src/Routes/Routes.jsx
        import { createBrowserRouter } from "react-router-dom";

         const router = createBrowserRouter([
          {
            path: "/",
            element: <div>Hello world!</div>,
          },
         ]);

     export default router;
