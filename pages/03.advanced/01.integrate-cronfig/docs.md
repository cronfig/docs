---
title: 'Integrate Cronfig'
taxonomy:
    category:
        - docs
---

Cronfig was built to be simple. You probably know that by now. But it is also very simple to integrate anywhere. All you need is some HTML page you can paste some Javascript and configure it for your app with a Javascript object. No server-side magic needed.

<script src="https://gist.github.com/escopecz/f398baa387173147aefc1a3cf82fa084.js"></script>

### What's happening on the interesting lines

#### Line 4,5,6

A `div` with `id="cronfig-wrapper"` is where the Cronfig JS will render its content. You can type in `loading...` or paste in a spinner to tell the user the content is coming soon.

#### Line 8

Add the `cronfigConfig` object to `document` to integrate Cronfig with needs of your app.
