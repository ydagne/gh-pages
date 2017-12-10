---
layout: post
title: Web Application 101
excerpt: "An introduction to web applications"
categories: blog
tags: [python, web]
image:
  feature:
  credit: 
  creditlink:
comments: true
share: true
modified: 2017-12-03T14:11:53-04:00
---

In order to deploy a dynamic web site on a server machine, one needs an operating system, an HTTP server, a database, and a server-side engine that interacts with the database and processes requests that come from clients (web browsers). There are three commonly used alternative protocol stacks (combination of web servers, frameworks and platforms). These stacks are based on the three most popular HTTP servers:

- [Apache](https://www.apache.org)
- [Node.js](https://nodejs.org/en/) and
- [Rails](http://rubyonrails.org/)

## LAMP Stack

LAMP is an acronym for **L**inux operating system, [**A**pache](https://www.apache.org) HTTP Server, [**M**ySQL](https://www.mysql.com/) relational database and [**P**HP](http://www.php.net/) programming language. Since Apache, MySQL and PHP can run on other platforms such as Windows, there are also some variants LAMP stack. WAMP stack, which is based on Windows operating system, is one of them. PHP powers back-end (server-side) functionalities such as handling HTTP requests, and iteracting with MySQL database. The front-end is mainly implemented using HTML and javascript.

## MEAN Stack

MEAN stands for [**M**ongoDB](https://www.mongodb.com/) database, [**E**xpress](http://expressjs.com/) javascript-based web framework, [**A**ngularJS](https://angularjs.org/) front-end framework, and [**N**ode.js](https://nodejs.org/en/) HTTP server. Node.js is a JavaScript runtime built on [Chrome's V8 JavaScript engine](https://developers.google.com/v8/). Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient. Morever, since both the front-end and the back-end are powered by javascript, it simplifies web development process.

## Ruby on Rails

[Rails](http://rubyonrails.org/) is a complete web application development framework written in [Ruby](https://www.ruby-lang.org/en/) language. It is designed to make programming of web applications easier by making assumptions about what every developer needs to get started. It abstracts routine works and allows you to write less code while accomplishing more than many other languages and frameworks.