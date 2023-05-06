# Class 7 Reading Notes

## Intro to Node.js on sitepoint.com

- V8 engine is enhanced with file system API, HTTP library and operating system related utility methods. Created by Ryan Dahl.

- An npm version manager allows you to install multiple versions of Node and switch between them at will and lets you set a Node version on a per-project basis.

- npm = largest software registry


1. What is node.js?

- An asynchronouse event based JavaScript runtime designed to build network applications.

- If you want to devlop apps with a JS framework like React, you need working knowledge of Node and npm because these frameworks are available via npm and rely on Node to create development environment in which they can run.

2. In your own words, what is Chrome’s V8 JavaScript Engine?

- The V8 engine is a JavaScript engine that powers Google Chrome and runs the JavaScript code that we write.

3. What does it mean that node is a JavaScript runtime?

- Node is a program that can be used to execute JS on a computer.

4. What is npm?

- A package manager that comes bundled with Node. npm stands for Node Package Manager and it is a library for JavaScript software packages and comes with command-line tools that help install these packages.

5. What version of node are you running on your machine?

- v19.8.1

6. What version of npm are you running on your machine?

- 9.5.1

7. What command would you type to install a library/package called ‘jshint’?

- npm install -g jshint will install the jshint package globally on your system.

8. What is node used for?

- If you want to devlop apps with a JS framework like React, you need working knowledge of Node and npm because these frameworks are available via npm and rely on Node to create development environment in which they can run. Node is also used to run JavaScript on the server.

-  Node is suited for apps that require real-time interaction or collaboration (ex. chat sites, Google Docs(can be shared and edited in real time from multiple users)). Also good for buiding APIs and sites that involve data streaming

- Node.js is single threaded and event driven meaing everything that happens in Node is a response to an event. If a request is blocked by I/O operation while a new request comes in, instead of waiting for the first request to complete, it will run a callback before continueing to the next event and then finish the original request when the I/O operation is finished. Node uses libuv to implement this non-blocking behavior (asynchronous)

## 6 Reasons for Pair Progamming

1. What are the 6 reasons for pair programming?

- Greater efficiency
- Enganged collaboration
- Learning from fellow students
- Social skills
- Job interview readiness
- Work environment readiness

2. In your experience, which of these reasons have you found most beneficial?

- Learning from other students has been the most beneficial reason for pair programming. It is often times super helpful to get someone else's perspective on a problem or project to help me grow my skills and understanding.

3. How does pair programming work?

- Pair programming involves a driver and a navigator. The driver types the code and the navigator guides the driver with their words. 