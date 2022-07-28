# Rest API Tutorial - Part 1

This tutorial aims to create a complete Node.js based RESTful API. Its purpose is to be self-explanatory, using especially code comments to achieve that.

It's good to mention that a previous knowledge on JavaScript basics is important for the right understanding of this tutorial.

Besides, it's not necessary to have a previous knowledge on Node.js, since we'll be covering the basics here.

## Index

* [First Part Goal](#first-part-goal)
* [How to Use this Tutorial](#how-to-use-this-tutorial)
* [Resources](#resources)
* [Getting Started](#getting-started)
* [How did we do it?](#how-did-we-do-it)
* [What Comes Next?](#what-comes-next)

## First Part Goal

With this first part, our goal is to be able to say "Hello World" to anyone who calls our API. It's a useful though simple achievement to start this development process.

## How to Use this Tutorial

You can make a good use of this tutorial by setting it up (see [Getting Started](#getting-started) section), reading the [How did we do it?](#how-did-we-do-it) section and reading the code comments.

While reading the [How did we do it?](#how-did-we-do-it) section, it's an interesting idea to switch between your browser and your code editor, so you can follow the steps we took directly inside the code.

## Resources

To make it happen, this project uses the following external resources:

- `Visual Studio Code`: We're using Visual Studio Code as code editor and command line tool. For details, please visit https://code.visualstudio.com/
- `Express.js`: Used as the basic structure of our API. For details, please visit https://expressjs.com/
- `Nodemon`: Used for debugging purposes. For details, please visit https://www.npmjs.com/package/nodemon

## Getting Started

In order to get started with this tutorial, make sure **you have Node.js installed in your machine** (for details, please visit https://nodejs.org/en/download/) and a **code editor** available (we're using Visual Studio for this project, but it's up to you to choose one).

With all this in place, you can move on.

1. Download the project files and place them into a directory of your choice. You can also use the `git clone` tool if you prefer to.

2. Using a terminal (Visual Studio Code has a built-in terminal, which can be accessed pressing `ctrl + '`), navigate to the folder you've placed the files and type `npm install` and press Enter. This will install all the external modules we will be using in this tutorial.

3. Still in the terminal, type `npm start` and press Enter. This will run the application so you can see it working.

4. Go to your browser and access the address http://localhost:3000/. If you see the phrase "Hello World!", you're done with the setup. Now go to the [How did we do it?](#how-did-we-do-it) section to start learning.

## How did we do it?

To produce this simple result you've seen in the [Getting Started](#getting-started) section, we went through some steps. Here are them:

1. Inside an empty folder, we started the **npm packager** by navigating into this folder in the terminal and running `npm init`. This command makes the terminal to ask us about details of our project, which we can answer accordingly. Usually, you can just press Enter to each question, which makes you use the default answer, but in this case we filled the form with some details of the tutorial. If you plan to replicate this process, you can stick to the default answers, and it'll be working in the same way.

2. Still in the terminal, we ran the command `npm install express nodemon` to install the dependencies we've mentioned in the [Resources](#resources) section.

3. On the project tree, we created a new folder called `src` and inside of it, we created a file called `index.js`.

4. In the file `index.js`, we wrote the code you can check in this same file in this tutorial, and saved it. Remember to read the comments in the file, so you can understand what's going on over there.

5. We taught `npm` what would be the "start" of our API by adding the property `"start": "nodemon src/index"` in the "scripts" property, inside the `package.json` file. Usually, to start a Node.js application, we can just run `node file.js` in the terminal. In this case, we're doing a little bit different:
    - First, we are not typing the execution command in the terminal, but in the `package.json` file. We do this way for clarification purposes, so we can run the command `npm start` in the terminal instead of any complex execution command we may need to start our server. This is neat and simpler.
    - Second, we're using the **nodemon** tool (the one we've installed in the step 2), which makes the execution of the file restart after any changes in it or other .js files in the project. This is done for debugging purposes.

With all this in place, we just run `npm start` in the terminal and enjoy our API.

## What Comes Next?

Now we have an up and running API, but it actually just say "hello". So adding some more real world capabilities to it will be our next step.

#### Other Parts Links:
- [Part 2](https://github.com/lucas-gustavoc/rest-api-tutorial-step2)
- [Part 3](https://github.com/lucas-gustavoc/rest-api-tutorial-step3)
- [Part 4](https://github.com/lucas-gustavoc/rest-api-tutorial-step4)
