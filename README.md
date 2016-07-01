# Introduction to Node

## Overview

We'll give a quick overview of Node.js and explain non-blocking I/O, and provide a bird's eye view on how it fits into web development.

## Objectives

1. Describe increase in performance when using Node.js?
1. Describe the re-use of code when using Node.js?
1. Describe Node.js history (a very brief version)

## Non-Blocking Input/Output

Have you ever worked with Rails and had to wait while ActiveRecord was processing some simple database join? Or maybe you remember seeing the fail whale every time Twitter was over capacity. It's happened quite often, maybe every week. Slow systems are not only frustrating to users, but also to companies. They cost companies money because users leave them for other services and products. A slow system is a system that cannot handle the traffic or load properly. The term "slow" is relative. For example. what we consider slow in 2016 is very fast compared to 2000. With Rails the slowness is due to the high-level of abstraction which means that the Object Relational Mapper (ORM) Active Record and the framework as a whole is doing too many things. It's a good thing for developers because we have to code less, but as real-life shows, it's not so good for the systems. Another reason for slowness is the architecture of the system.

![](fail-whale.gif)


Slow platforms are not just annoying to develop with but they also cost companies hundreds of thousands of dollars each month in servers and CPUs. What if we told you there is a high performing and scalable system which is extremely efficient yet fun to work with?

Node.js is one of those scalable platforms which enable engineers to build fast systems. Imagine a Starbucks coffee shop. You see 20 people standing in line and just one person working at the cafe. The single barista is also a cashier meaning this employee must first take the order, then make it. Each person has to wait for the not only for his or her drink but for the order before them... would you wait in line if you were the last person? The 20th person? As a manager of this cafe, the only way to scale is to add more registers. By adding more registers and employees we can have more than one line. Each cashier is still taking the orders and making the drinks. But this is not the most pleasant experience for customers because they would still be standing in a line. Slow systems are painful and they cost money because customers can walk away without ordering anything.

Luckily, this is not how the most Starbucks or coffee shops operate. You order your fancy choco-mocha-frappe-latte-soy-decafs, the cashier yells your order and takes your money. You step aside to check to work on some Learn.co lessons. You can now do other things while waiting for your drink. The line isn't blocked. It moves faster. The orders are taken by the cashier and the drinks are made by another employee. This is a more pleasurable experience than waiting the entire time in the line right?

The first scenario is how most platforms, including Rails, operate. The approach is called blocking input/output (I/O) in computer world because the line(s) are blocked by previous orders (or tasks in the computer lingo). The line is a metaphor for a queue of tasks while the employees can be servers. So how is Node.js different? Node.js has non-blocking I/O which as you might guess is the latter approach.

The queue moves, and the processes are executed asynchronously and without blocking the queue. Note: The real Starbucks uses blocking I/O for simple drinks like regular coffe and teas since they take very little time to make.  However, the chain uses a non-blocking I/O system for more complicated, hand-crafted drinks like lattes, frappes, Cappuccino and others that take longer to make.

Therefore, Node.js systems can serve more traffic because they are not idle or blocked. They can process other tasks while waiting on the input/output operations (usually the most time consuming). For example, a Node.js server can process a request from client B while it waits for a response from a database to server a response to client A. Most other systems will do nothing while they wait for a reply from a database to server client A's request.


## Full Stack JavaScript

When you develop applications in Rails, you might use Haml to render server-side templates and then on the client-side you might use another framework and another template engine like Angular. Those libraries are great, but consider that you have hundreds of pages with duplicate templates: one file for server-side rendering and another for browser rendering. To add complexity, this is an enterprise application which has been developed many years ago and you have 20+ people working on the project. How are you going to make changes to 200+ files? You need to make similar changes to two files and then change the tests as well. What if they are different languages? Imagine the nightmare. Sadly this is the case in most systems.

Node is different because it has this concept called full stack, isomorphic or universal JavaScript. No matter what you call it, the idea is that you can re-use files, libraries and modules between the server and the browser seamlessly. This is huge because as web developers, we've amassed boatloads of great utilities and tools for browser JavaScript. Most of them are ready-to-go in the Node environment with very minor modifications, e.g., using [Browserify](http://browserify.org). Same thing applies to books, blogs, and screencasts. JavaScript is continually being improved, (ES6, ES7, etc.) which puts Node in a unique position. 

## Node History

We know that you probably want to learn how to's and not so much about Node history so feel free to skip this part. Nevertheless, knowing Node history will make you a star at developer happy hours. So how did Node start?

1. 2009: Ryan Dahl invents Node to make file uploads easier. JavaScript is the third language of choice and it sticks. Ryan joins Joyent.
2. 2011: Isaac Schlueter writes npm (package manager); Windows version of Node.js is released. Versions 0.1 to 0.6 released.
3. 2012: Isaac Schlueter replaces Ryan Dahl as "head" of Node at Joyent. Versions 0.6 to 0.9 released
4. 2013: Versions 0.10 and 0.11 are released.
4. 2014: Timothy J. Fontaine becomes the Node project lead; Node.js is forked by open source community to speed up releases. Versions 0.12 released.
5. 2015: Node.js Foundation is created and io.js becomes Node.js. Versions 1.x through 5.x are released.

And this video which in 5 minutes explains [the past, present and the future of Node.js and Joyent](https://www.youtube.com/watch?v=dWwIHRLzLew).



## Resources

1. [The Story of the Fail Whale](http://readwrite.com/2008/07/17/the_story_of_the_fail_whale)
1. [Ryan Dahl: Original Node.js presentation](https://www.youtube.com/watch?v=ztspvPYybIY)
1. [The past, present and the future of Node.js and Joeynt](https://www.youtube.com/watch?v=dWwIHRLzLew)
4. [Node.js Foundation](https://nodejs.org/en/foundation)

---

<a href='https://learn.co/lessons/node-overview' data-visibility='hidden'>View this lesson on Learn.co</a>
