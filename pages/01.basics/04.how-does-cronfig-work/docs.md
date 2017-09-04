---
title: 'How does Cronfig work'
---

Mautic needs to be poked periodically so it could perform background tasks which does the automation tasks like executing campaign actions in the right time or tasks which would take too long to perform when clicking in the UI like import or email sending. But you already know that and that's why you are interested in Cronfig.

1. When you install the Cronfig plugin to your Mautic it will allow you to create a new account and tasks which you want to execute periodically.
2. The information will get stored into database server.
3. A worker is periodically checking if there is some task which should be triggered at the moment.
4. If there is some, it will create a HTTP call to the Cronfig plugin installed in your Mautic.
5. Cronfig plugin will trigger the task similarily like you would do executing the command via CLI.
6. Cronfig worker waits for certain time for a response of the command. If there is, it will store it to Cronfig database server so you could view it in the Cronfig plugin user interface or get notified if it fails for several times in the row.