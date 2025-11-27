# moringa-Capstone-Project-

#  **Beginner’s Toolkit with GenAI: Build Your First Node.js + Express API Server (Step-by-Step Guide)**

Welcome to the **Beginner’s Toolkit with GenAI**!
This guide teaches **complete beginners** how to build a very simple backend using **Node.js** and **Express** — starting from **nothing**.

You do NOT need any previous experience with backend development.
You only need:

* A laptop
* Internet
* Curiosity 😊
* And this guide (with GenAI support)

---

#  **What You Will Learn**

By following this toolkit, you will learn how to:

* Install Node.js
* Create a project folder
* Set up npm
* Install Express.js
* Write a tiny API
* Run it on your own machine
* Fix common errors
* Use GenAI (AI chatbot) to ask questions and solve problems

This is a simple, friendly introduction to backend development.

---

#  **Goal of This Toolkit**

The goal is to build a **very basic API** that returns:

```json
{ "message": "Hello World from Express!" }
```

This does NOT require advanced coding.
It’s meant to help beginners understand how servers work.

---

#  **Features of This Project**

* Easy to build
* Only one file of code
* Uses only one library: Express
* Works on any laptop
* Perfect for students and beginners
* Includes real AI prompts used during learning
* Includes simple troubleshooting

---

#  **Tools You Need**

| Tool                      | Why You Need It                       |
| ------------------------- | ------------------------------------- |
| **Node.js**               | To run JavaScript outside the browser |
| **npm**                   | To install packages (comes with Node) |
| **Express.js**            | To build the API                      |
| **VS Code (recommended)** | To write your code                    |
| **GenAI**                 | To help you learn and debug           |

---

#  **What We Will Build (Final Project Structure)**

```
my-express-api/
│
├── index.js        # Your main code file
├── package.json    # Created by npm automatically
├── package-lock.json
└── README.md       # Documentation
```

---

#  **STEP-BY-STEP: Build the Project From Scratch**

These steps assume you know **nothing** — and that’s perfect.
Let’s begin.

---

##  **Step 1: Install Node.js**

Go to:

👉 [https://nodejs.org](https://nodejs.org)

Download and install the **LTS version** (recommended for beginners).

After installation, open your terminal (Command Prompt, PowerShell, or VS Code terminal) and type:

```bash
node -v
npm -v
```

If you see version numbers, you're good to go!

---

##  **Step 2: Create a Folder for Your Project**

Open your terminal and run:

```bash
mkdir my-express-api
cd my-express-api
```

This creates an empty folder where your project will live.

---

##  **Step 3: Initialize npm (Creates package.json)**

This command tells Node.js to set up a new project:

```bash
npm init -y
```

You'll see a new file appear:

```
package.json
```

This file stores information about your project.
You don't need to edit it manually right now.

---

##  **Step 4: Install Express.js**

Express is the tool that lets us create servers easily.

Install it by running:

```bash
npm install express
```

npm will download Express into your project.

---

##  **Step 5: Create Your Server File**

Create a new file called:

```
index.js
```

Then put this code inside:

```javascript
// Load the express library
const express = require('express');

// Create an express app
const app = express();

// Create a route (homepage)
app.get('/', (req, res) => {
  res.json({ message: 'Hello World from Express!' });
});

// Tell the app which port to use
const PORT = 3000;

// Start the server
app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```

This is your entire backend.
Just a few lines of code!

---

##  **Step 6: Run Your Server**

In the terminal:

```bash
node index.js
```

If everything works, you will see:

```
Server running on http://localhost:3000
```

This means your backend is alive.

---

##  **Step 7: Open Your API in the Browser**

Go to:

👉 [http://localhost:3000](http://localhost:3000)

You should see:

```json
{ "message": "Hello World from Express!" }
```

CONGRATULATIONS!
You just built your first backend 🎉

---

#  **Beginner-Friendly Code Explanation**

Below is what each part of the code does:

---

### **1. Load Express**

```javascript
const express = require('express');
```

This brings Express into your project.

---

### **2. Create an App**

```javascript
const app = express();
```

This creates an application that can receive requests.

---

### **3. Create a Route**

```javascript
app.get('/', (req, res) => {
  res.json({ message: 'Hello World from Express!' });
});
```

This means:

* When someone visits the homepage (`/`)
* Send them the JSON message

---

### **4. Start the Server**

```javascript
app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```

This makes your server start listening for requests.

---

#  **AI Prompt Journal (What AI Helped With)**

### ✔ Prompt 1

“Explain Node.js and Express.js to a complete beginner.”

AI explained everything in simple language.

---

### ✔ Prompt 2

“Guide me step-by-step to build a simple Express API from scratch.”

AI helped structure this tutorial.

---

### ✔ Prompt 3

“I’m getting ‘Cannot find module express’. How do I fix it?”

AI suggested installing Express again using:

```bash
npm install express
```

---

### ✔ Prompt 4

“Write a beginner-friendly README for a GenAI toolkit.”

AI helped make everything clear and simple.

---

#  **Common Errors (Beginner Friendly Fixes)**

---

###  Error: Cannot find module ‘express’

**Reason:**
You didn’t install Express properly.

**Fix:**

```bash
npm install express
```

---

###  Error: Port already in use

**Fix:**
Change the port to another number:

```javascript
const PORT = 3001;
```

---

###  Nothing shows in the browser

**Fix checklist:**

* Did you run `node index.js`?
* Did you go to the correct link?
  👉 [http://localhost:3000](http://localhost:3000)

---

#  **References (Beginner Friendly)**

* Node.js → [https://nodejs.org](https://nodejs.org)
* Express.js → [https://expressjs.com](https://expressjs.com)
* W3Schools JavaScript → [https://www.w3schools.com/js](https://www.w3schools.com/js)
* MDN Web Docs → JavaScript Basics
* FreeCodeCamp → Node.js Tutorials

---

#  **Reflection: How GenAI Helped Me Learn Faster**

GenAI helped me:

* Understand new concepts in simple words
* Generate code examples
* Fix errors quickly
* Stay motivated
* Write documentation easily

GenAI acted like a friendly teacher guiding me at each step.

---

#  **Conclusion**

You have completed the **Beginner’s Toolkit with GenAI**!

You now know how to:

* Install Node.js
* Set up a new project
* Install Express
* Build a simple API
* Run it locally
* Use GenAI to support your learning

This simple project is the perfect first step into backend development.


