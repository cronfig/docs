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

#### Line 9

Specify `platform` name. For example type in _Mautic_ if you write another plugin for Mautic or _Wordpress_ if you integrate Cronfig with Wordpress.

#### Line 10 - 16

Specify what tasks can users start within Cronfig. This is key concept of Cronfig. You, as a developer, will configure the tasks for the app you are integrating with. You specify `url`, `title` and `description` for each task. Add multiple tasks if you need them. Users will simply enable those they want with one click. Simple.

>>>> Notice the example task URL. It has a **secret hash**. Use similar technique to secure potentially expensive trigger URLs.

#### Line 17

Cronfig is meant to use inside an app configuration. So your users should be logged in and you should know their **email address**. Fill it in so they doesn't have to type it in.

#### Line 18

If you know the API key of the users, fill it in here so it's pre-filled for them and they doesn't have to search for it in their inbox. How could you know that? Glad you asked! See line 19.

#### Line 19

This function will run when user filles in the API key. So you can easily catch it and store it to pre-fill it next time (line 18). Make lives of your users a bit easier.