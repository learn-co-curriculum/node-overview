# Introduction to Node.js

## Overview

We'll give a quick overview of Node.js and explain non-blocking I/O, and provide a bird's eye view on how it fits into web development.

## Objectives

1. Describe increase in performance when using Node.js?
1. Describe the re-use of code when using Node.js?
1. Describe Node.js history (a very brief version)

## Non-Blocking Input/Output

Have you worked with Rails and had to wait while ActiveRecord was processing some simple database join? Or maybe you remember seeing the fail whale every time Twitter was over the capacity. It happened quite often, maybe every week. Slow systems are not only frustrating to users, but also to companies. They cost money to companies because users leave to other services and products. A slow systems is a system that cannot handle the traffic or load properly. The term "slow" is relative. For example. what we consider slow in 2016 is very fast comparing to 2000. A reason for a slow application can be the use of a bad architecture. With Rails the slowness is due to the high-level of abstraction meaning the Object Relational Mapper (ORM) Active Record and the framework as the whole is doing too many things. It's a good thing for developers because we have to code less, but as real-life showed, not so good for the systems. Another reason for slowness is the architecture of the system.

![](fail-whale.gif)


Slow platforms are not just annoying to develop with, they also cost companies hundreds of thousands of dollars each month in servers and CPUs. What if we told you there is a high performing and scalable system which is extremely efficient yet fun to work with?

Node.js is one of those scalable platforms which enable engineers to build fast systems. Imagine a Starbucks coffee shop. You see 20 people standing in line and just one person working at the cafe. The single barista is also a cashier meaning this employee must first take the order, then make it. Each person has to wait for the not only for his or her drink but for the order before them... would you wait in line if you are the last? The 20th person? As a manager of this cafe, the only way to scale is to add more registers. By adding more registers and employees we can have more than one line. Each cashier is still taking the orders and making the drinks. This is not the most pleasant experience for customers because they don't like standing in lines. Slow systems are painful and they cost money because customers can walk away without ordering anything.

Luckily, this is not how the most Starbucks or coffee shops operate. You order your fancy choco-mocha-frappe-latte-soy-decafs, the cashier will yell your order and take the money. You step aside to check to work on some Learn.co modules. You can do other things while waiting for your drink. The line is not blocked. It moves faster. The orders are taken by the cashier and the drinks are made by another employee. This is a more pleasurable experience than waiting the entire time in the line right?

The first scenario is how most of the platforms, e.g., Rails operate. The approach is called blocking input/output (I/O) in computer world because the line(s) are blocked be previous orders (or tasks in the computer lingo). The line is a metaphor for a queue of tasks while the employees can be servers. So how Node.js is different? Node.js has non-blocking I/O which as you might guess is the latter approach.

The queue moves, and the processes are executed asynchronously and without blocking the queue. Note: The real Starbucks uses blocking I/O for simple drinks house brews in a big coffers like Pike Place (regular brew) and teas. They take a minute or so to make.  However, the chain uses a non-blocking I/O system for hand-crafted one like lattes, frappes, Cappuccino and others which take longer to make.

Therefore, Node.js systems can serve more traffic because they are not idle or blocked. They can process other tasks while waiting on the input/output operations (usually the most time consuming). For example, a Node.js server can process a request from a client B while it waits for a response from a database to server a response to client A. Most other system will do nothing while they wait for a reply from a database to server client A's request.


## Full Stack JavaScript

When you develop application in Rails, you might use Haml to render server-side templates, then on the client-side you might use another framework and another template engine like Angular or Mustache. Those libraries are great, but consider that you have 100s of pages with a duplicate templates: one file for server-side rendering and another for browser rendering. To add complexity, this is an enterprise application which has been developed many years ago and you have 20+ people working on the project. How are you going to make changes to 200+ files? You need to make similar changes to two files and then change the tests as well. What if they are different languages? Imagine the nightmare. Sadly this is the case in most systems.

Node is different because it has this concept called full stack, isomorphic or universal JavaScript. The term "full-stack is the most descriptive of the powers of node. No matter what you call it, the idea is that you can re-use files, libraries and modules between server and browser seamlessly. This is huge because we, as web developers, amassed boatloads of great utilities and tools for browser JavaScript. Most of them are ready-to-go in Node environment with very minor modifications, e.g., using [Browserify](http://browserify.org). Same thing applies to books, blogs, screencasts. JavaScript is continually improved, (ES6, ES7, etc.) which put Node in a unique position. Honestly, we doubt Go or some other new platform can compete with Node in near future because of this unique combination which allows developers to have language to rule 'em all!

## Node History

We know that you probably want to learn how to's and not so much about Node history. Feel free to skip this part. It won't be in the test. ;) Nevertheless, knowing Node history will make you a start at developer happy hours. So how did Node start?

1. 2009: Ryan Dahl invented Node to make file uploads easier. JavaScript was the third language of choice and it stuck. Ryan joined Joyent.
2. 2011: Isaac Schlueter wrote npm (package manager); Windows version of Node.js was released. Versions 0.1 to 0.6 released.
3. 2012: Isaac Schlueter replaced Ryan Dahl as "head" of Node at Joyent. Versions 0.6 to 0.9 released
4. 2013: Versions 0.10 and 0.11 released.
4. 2014: Timothy J. Fontaine became the Node project lead; Node.js is forked by open source community to speed up releases. Versions 0.12 released.
5. 2015: Node.js Foundation is created and io.js becomes Node.js. Versions 1.x through 5.x released.

Watch this video which in 5 minutes explains [the past, present and the future of Node.js and Joeynt](https://www.youtube.com/watch?v=dWwIHRLzLew).



## Resources

1. [The Story of the Fail Whale](http://readwrite.com/2008/07/17/the_story_of_the_fail_whale)
1. [Ryan Dahl: Original Node.js presentation](https://www.youtube.com/watch?v=ztspvPYybIY)
1. [The past, present and the future of Node.js and Joeynt](https://www.youtube.com/watch?v=dWwIHRLzLew)
4. [Node.js Foundation](https://nodejs.org/en/foundation)

---

<a href='https://learn.co/lessons/node-overview' data-visibility='hidden'>View this lesson on Learn.co</a>
