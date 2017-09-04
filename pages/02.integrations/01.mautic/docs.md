---
title: Mautic
published: true
---

### Installation

1. [Download](https://cronfig.mautic.net/asset/1:mautic-cronfig-plugin) the plugin
2. Unzip the downloaded package.
3. Upload the unzipped folder to the plugins folder and rename it to CronfigBundle the way you could locate CronfigBundle.php file on this path: plugins/CronfigBundle/CronfigBundle.php.
4. Clear Mautic's cache. Either run app/console cache:clear command in the Mautic's root dir or simply delete the content of app/cache dir.
5. Go to the right hand side Mautic menu (click the cog icon in the top right corner to slide the menu out) and go to Plugins.
6. Click the Install/Upgrade Plugins button. The Cronfig icon should appear in the list of plugins.
7. Go to the right hand side Mautic menu again. A new menu item called Cronfig should be there. Hit it. A register/login screen should appear.
8. Your email should be prefilled. Click on the Register button and check your email inbox. Your API key should appear in your inbox any second.
9. If you received the Cronfig registration email, copy the API key from it, insert it to the Log in input and log in.