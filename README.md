# Banking-app-structure
Structure for The Kenya Bankers Vite-React Frontend App


**How to start Vite-React Project**
- npm create vite app --template react
- cd app
- npm install
- npm run dev
-  in src folder create pages, styles and components folder
-  add images to public folder
-  kill terminal
-  install tailwind css
-  remove unwanted codes, files, and folders

**How to deploy it on hostinger**
- npm run build
- dist folder is created
- copy folder into public_html in hostinger
- add .htaccess file in public_html

**Structure defintions**
Public folder: used for static assets e.g images, etc. that don't need processing by the build tool. Files in this folder are directly accessible and won't be processed by Vite. One can call images in .jsx files without having to import it as a component e.g "<img src="/ats_website/raleigh.jpg" alt="Me" className="object-cover w-full h-full" " /> if they are stored there.

Src folder: where the application's source code resides. It includes all the JavaScript/JSX, CSS, and other files that need to be processed and bundled by Vite.

index.html: where one can add the favicon, and webapp/website title, it contains the entry point of the vite project e.g. main.jsx

tailwind.config.js: if using tailwind css, one can define screen size values here using theme as a property

src/components: .jsx files that need to be imported to pages. Components hold the exact content and styles for the webapp/website e.g text, text cells, etc.

src/pages: components are imported here. pages are .jsx files too

src/styles: contains custom css stylesheet e.g global.css, which is imported in main.jsx

src/App.jsx: imports pages, contains path names definitions in routes, and the 'scroll to the top' component

src/index.css: holds tailwind's base, components and utilities

src/main.jsx: imports index.css, global.css (custom stylesheet), App.jsx, BrowserRouter, ReactDom, called in the root defined in index.html i.e main.jsx, is enclosed in BrowserRouter
