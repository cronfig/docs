---
title: 'Integrate Cronfig administration into any app'
taxonomy:
    category:
        - docs
---

Cronfig was built to be simple. You probably know that by now. But it is also very simple to integrate anywhere. All you need is some HTML page you can paste some Javascript and configure it for your app with a JSON object. No server-side magic needed.

```html
<div id="cronfig-wrapper">
    Loading...
</div>
<script type="text/javascript">
    document.cronfigConfig = {
        platform: 'app_name',
        tasks: {
        	{
        		url: 'https://yourapp/trigger/action?secret=slkj23ori2kln',
                title: 'Trigger the action'
                description: 'Makes your app to do this and that',
        },
        email: 'known@user.email',
        apiKey: 'known_api_key_here',
        rememberApiKey: function(apiKey) {
            // AJAX call to save/remember filled in API key 
            // so user does not have to enter it every time
        }
    }
</script>
<script type="text/javascript" src="https://cdn.cronfig.io/cronfig.js"></script>
```
