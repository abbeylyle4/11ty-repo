---
title: Introduction to JavaScript and Open Web Components.
description: This is a post on My Blog about JavaScript and Web Components.
date: 2022-02-23
tags:
  - another tag
layout: layouts/post.njk
---
Maybe you're also a beginner, or have no experience with JavaScript and are looking for a place to start. Welcome! We will be going through the steps for making sure that you have all you need to begin your web dev journey. 

_These steps will be most compatible with Mac users_

## What is JavaScript?

JavaScript first appeared in 1995 as a scripting language for the World Wide Web. It operates alongside HTML and CSS to increase interactivity and functionality on web pages. Nowadays, over 97% of websites use JavaScript to increase capabilities on their client-facing interfaces.

Now that you have a brief background, let's get started with getting all the tools we need.

## VS Code
VS code is a code editing software that comes in handy when learning JavaScript. It provides support for debugging and version control. It is a great option for beginners who are getting into web dev. 

You can get VS Code [here](https://code.visualstudio.com/Download)

## NodeJS
NodeJS is an open source platform and allows you to run server-side applications on your personal machine.

When [downloading](https://nodejs.org/en/download/), make sure that you download the LTS/"recommended for most users" option for a more reliable platform.

**Tip**: to double check that NodeJS has installed successfully, you can simply type `node` in your terminal window (for macOS users, you can navigate to it by searching 'terminal' in your launchpad)
![NodeJS](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/y6jj36msd5kkylkrjghr.png)
  

### npm
Luckily for you, npm (node package manager) is installed as a _package deal_ with NodeJS. Npm is the default package manager for NodeJS and allows you to use third party code in your own. It is one of the largest software registries, giving you a plethora of tools for your own code.

Similarly to NodeJS, you can ensure you have npm by typing `npm` in your terminal window. You will see a longer message this time showing some of the capabilities you have with npm!![npm](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6qxrp0uql2cgxmb4l261.png)

## Git

Git is a version control service used for communicating and collaborating between different programmers creating code for one project.

You can get git [here](https://git-scm.com/downloads).
After completed, type `git` in terminal to ensure correct installation.

---


## Open Web Components
Now that we have all the necessary tools to begin, let's work on creating our own web component! First, we must create a new folder in Finder to host this project. Then, return to your terminal window and navigate to that folder you just created. You can do this by typing `cd "foldername"`. 
**Tip**: Make sure you are using the whole file path, typing just the destination folder can run an error.

Once in your folder, code `npm init @open-wc` and run the command. This initializes the process for us to create our first web component!
![open wc](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mzogl69k19q38er44yc8.png)

From here, we answer the following prompts:
1. Scaffold a new project
2. Web component
3. Press `a` to select all options, then `enter` to run
4. Deny typescript
5. Pick a name for your first project! (I picked "hello-world")
![creating wc](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/6udxmnyy3y576p9wcv1t.png)  
6. Select yes to writing file structure to disk
7. Install dependencies with npm (this may take some time)
 
After receiving the message that we are all set up, simply follow the two commands to run your web server. You should be taken to your first web component!
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t1ou9sje23z39w49smya.png)

---

## Understanding your Web Component

Once the web component is created, it is important to understand how it even operates using the `src/HelloWorld.js` file. In src files, you are able to edit code to enhance components of the websites as I mentioned at the beginning of this post. The src file looks something along the lines of this:

![src](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/n4rbe39eixl1eq2ss9up.png)
 
You can see at the beginning of the code, LitElement is being imported. Lit supports the building of fast and lightweight web components. In order to get more familiar with Lit, I recommend following this [tutorial](https://lit.dev/tutorial/). 
