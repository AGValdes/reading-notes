# Node.js

- Node is built on **Chrome's V8 JavaScript Engine**
- The V8 engine is am open-source JavaScript engine
- Node programs are not executed in the browser.
-  the creator of Node (Ryan Dahl) took the V8 engine and enhanced it with various features, such as a **file system API**, an **HTTP library**, and a number of operating system–related **utility methods**.
- Node supports modern JS syntax
- **npm** is a package manager included in Node.
- you can install packages **globally** and **locally**
- `npm init -y` will create and auto-populate a **package.json** file in the same folder
- node-modules folder should not be included in version control, instead: if you open the package.json file, you’ll see node modules in the **dependencies field**.
- By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use `npm to install` whatever packages it needs to run.
### Node.js is used for:
- **installing** (via npm) and **running** (via Node) various **build tools** — designed to automate the process of developing a modern JavaScript application.
- running JavaScript on a **server**
- **event-driven** which means that everything that happens in Node is in reaction to an event.
- Node’s execution model causes the server very little overhead, and consequently it’s capable of handling a large number of simultaneous connections.
- Node is particularly suited to building applications that require some form of real-time interaction or collaboration
### Advantage:
- You can do everything in the same language, you can easily share code between the server and the client.
-  it speaks JSON
- JavaScript is ubiquitous: most of us are familiar with JavaScript, or have used it at some point.

![NodeImage](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)

[<-- Back](301readingnotes.md) [Back to Home](README.md)
