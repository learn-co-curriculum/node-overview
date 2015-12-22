# Quick Overview and Introduction to Node.js

## Overview

## Objectives

1. Describe the definiton of what is Node
1. Describe Node as a non-blocking I/O platform
1. Explain key differences between Node and other platforms like Java, Ruby, and Python
1. Describe Node history (a very brief version)
1. Get the sense of how Node fits into web development
1. Describe how Node fits into other development environments (embedded systems, IoT, drones)
1. Describe Node non-blocking I/O on a coffeeshop metaphor
1. Describe Node ecosystem, npm, its philosyphy of granular modules and its benefits

## What is Node.js

Node.js is a non-blocking platform for building web applications. It uses JavaScript, or to be more precise ECMAScript (ES) with JavaScript being one implementation of ES and Node another. While Node started as a web platform, it quickly found applications in other areas such as build tools, package managers code generators, embedded systems and more.

## Non-blocking I/O


## Node vs Others

One of the key differences between Node and other platforms such as Java, Ruby and Python is its non-blocking I/O. Some other platforms/languages have frameworks to achieve non-blocking I/O, e.g., [Netty](http://netty.io), [EventMachine](http://rubyeventmachine.com) and [Twisted](https://twistedmatrix.com)

## Non-blocking I/O Metaphor

One of the biggest advantages of using Node.js over Python or Ruby is that Node has a non-blocking I/O mechanism. To illustrate this, let me use an example of a line in a Starbucks coffeeshop. Let's pretend that each person standing in line for a drink is a task, and everything behind the counter — cashier, register, barista — is a server or server application. Whether we order a cup of regular drip coffee, like Pike Place, or hot tea, like Earl Grey, the barista makes it. The whole line waits while that drink is made, and each person is charged the appropriate amount.

Of course, we know the aforementioned drinks (a.k.a., time-consuming bottlenecks) are easy to make; just pour the liquid and it's done. But what about those fancy choco-mocha-frappe-latte-soy-decafs? What if everybody in line decides to order these time-consuming drinks? The line will be held up, and in turn, grow longer and longer. The manager of the coffeeshop will have to add more registers and put more baristas to work (or even stand behind the register him/herself).

This is not good, right? But this is how virtually all server-side technologies work, except Node.js, which is like a real Starbucks. When you order something, the barista yells the order to the other employee, and you leave the register. Another person gives their order while you wait for your state-of-the-art eye-opener in a paper cup. The line moves, the processes are executed asynchronously and without blocking the queue.

This is why Node.js blows everything else away (except maybe low-level C++) in terms of performance and scalability. With Node.js, you just don't need that many CPUs and servers to handle the load.





<a href='https://learn.co/lessons/ruby-arguments-readme' data-visibility='hidden'>View this lesson on Learn.co</a>
