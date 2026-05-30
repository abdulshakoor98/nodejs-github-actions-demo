# Node.js GitHub Actions Demo

## Overview

This is a simple Node.js and Express application created to learn GitHub Actions CI/CD.

The project demonstrates how to:

* Create a basic Node.js application
* Install dependencies using npm
* Push code to GitHub
* Configure a GitHub Actions workflow
* Automatically run a build process on every push to the main branch

---

## Project Structure

```text
nodejs-github-actions-demo/
│
├── app.js
├── package.json
└── .github/
    └── workflows/
        └── build.yml
```

---

## Prerequisites

Before starting, make sure the following software is installed:

* Node.js
* npm
* Git
* Visual Studio Code

Check installation:

```bash
node -v
npm -v
git --version
```

---

## Step 1: Create Project

Create a new folder:

```bash
mkdir nodejs-github-actions-demo
cd nodejs-github-actions-demo
```

Initialize npm:

```bash
npm init -y
```

Install Express:

```bash
npm install express
```

---

## Step 2: Create Application

Create a file named:

```text
app.js
```

Add your Express application code.

Run the application:

```bash
node app.js
```

Open:

```text
http://localhost:3000
```

---

## Step 3: Add Build Script

Update package.json:

```json
"scripts": {
  "start": "node app.js",
  "build": "echo Build Successful"
}
```

Test build:

```bash
npm run build
```

Expected output:

```text
Build Successful
```

---

## Step 4: Configure GitHub Actions

Create folders:

```text
.github/workflows/
```

Create:

```text
build.yml
```

Add a workflow that:

1. Checks out repository code
2. Installs Node.js
3. Installs dependencies
4. Runs npm build

---

## Step 5: Push to GitHub

```bash
git init
git add .
git commit -m "Initial Commit"
git branch -M main
git remote add origin YOUR_REPOSITORY_URL
git push -u origin main
```

---

## GitHub Actions Workflow

Every time code is pushed to the main branch:

* GitHub creates a runner
* Installs Node.js
* Installs project dependencies
* Executes the build command
* Reports success or failure

---

## Learning Outcomes

After completing this project, you will understand:

* Basic Node.js project structure
* npm package management
* Git fundamentals
* GitHub repository management
* GitHub Actions workflow creation
* Continuous Integration (CI) basics

---

## Author

Abdul Shakoor

Learning Cloud, DevOps, Git, GitHub Actions and CI/CD.
