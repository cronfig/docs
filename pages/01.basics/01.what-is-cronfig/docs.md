---
title: 'What is Cronfig'
---

Cronfig is **simple** micro service breathing live to projects like [Mautic](https://mautic.org). Whenever you need to trigger an app periodically, Cronfig is the solution.

### The name

The name **Cronfig** is connection of the words **cron** and **fig**. Those words together gives an anagram of the word **config**, short for configuration. [Cron](https://en.wikipedia.org/wiki/Cron) (from Greek chronos which means time) is the software utility, a time-based job scheduler in Unix-like computer operating systems typically used to automate maintanance or administration. Fun fact; [fig sign](https://en.wikipedia.org/wiki/Fig_sign) is used in USA, UK or Czech Republic to pretend to "steal" someone else's nose as a game for small children. Do not use the fig sign in Germany or Italy, though. It has entirelly different meaning.

### Technologies used

The underlying architecture of Cronfig is built using the modern *best in class* technologies to fulfill the simplicity, speed and power which is the goal for the whole project.
- [NodeJS](https://nodejs.org) - server side non-blocking javascript runtime built on Chrome's V8 JavaScript engine takes care of the API.
- [MongoDB](https://www.mongodb.com) - NoSQL database built for fast and stable data querying and manipulation.
- [ReactJS](https://facebook.github.io/react) - Facebook's JS library for building user interfaces on top of virtual DOM.

Maybe you noticed that the whole service is built with one language, Javascript. Even the database is partially written in Javascript and use JSON (JavaScript Object Notation) as the format to store documents.

### The need for Cronfig

There was and still is the single pain point for Mautic users and that was setting up the Cron so Mautic could to its automation magic. The problem is that
- Every operation system have different way how to configure cron jobs.
- Every web hosting have different way how to configure cron jobs.
- Some web hostings doesn't offer this option at all.
- Some web hostings let their users to run jobs only once per hour, which isn't frequent enough.
- Each server can have the web root folder in a different location

The points above shows why it's not possible to write documentation for every single server or service where you can install Mautic. The Cronfig author was feeling the pain while helping Mautic community in the forums and decided to build a simple service which would work for all environments. The service which is simple to install into Mautic, simple to register and log into. The service which will gives you visibility into when and what jobs gets triggered, how long the execution takes and what is the result. The service which will let you know if there is something wrong with your Mautic or your server.