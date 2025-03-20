# SIT737 – Abhishek Srinivasan – S223750107

## Serving a Simple HTML Page with Node.js and Express

### Introduction
This document provides step-by-step instructions on how to create a simple web server using Node.js and the Express framework to serve an HTML response.

### Prerequisites
Before starting, ensure you have the following installed on your system:

- Node.js
- npm (Node Package Manager, included with Node.js)

### Step 1: Initialize the Project
1. Open a terminal and navigate to the project directory.
2. Run the following command to initialize a Node.js project:

   ```sh
   npm init -y
   ```
   
   This will generate a `package.json` file.

### Step 2: Install Express
To install Express, run:

```sh
npm install express
```

This will download and add Express to your project.

### Step 3: Create the Server File
1. Create a new file named `server.js` in the project directory.
2. Add the following code to `server.js`:

   ```javascript
   var express = require('express');
   var app = express();

   app.get('/', function (req, res) {
       res.send('Hello world');
   });

   app.listen(3000, () => {
       console.log('Server is running on http://localhost:3000');
   });
   ```

### Step 4: Run the Server
To start the server, run the following command in the terminal:

```sh
node server.js
```

If everything is set up correctly, you will see output similar to:

```sh
Server is running on http://localhost:3000
```

### Step 5: View the Web Page
1. Open a web browser.
2. Go to `http://localhost:3000`.
3. You should see the message **"Hello world"** displayed.

### Conclusion
This documentation covers how to create a basic web server using Node.js and Express to return a simple text response.

### GitHub Repository
[Project Repository](https://github.com/Abhishek-S-28/sit323_737-2025-t1-prac2p)
