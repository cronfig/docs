---
title: Mautic
published: true
---

### Installation

There are 2 ways to do it. If you have SSH access to your server or if you have only SFTP access. Follow the steps based on what you have.

#### I have SSH access

1. Log in with `ssh user@host`.
2. Go to your Mautic root folder and then to the plugins folder. `cd /path_to_mautic/plugins`
3. Download the zip package of the plugin and name it cronfig.zip. `curl https://github.com/cronfig/mautic-cronfig/archive/master.zip -o cronfig.zip -L` (`wget` can be used instead of `curl`)
4. Make sure the zip file appeared. `ls | grep cronfig` should return line `cronfig.zip`
5. Unzip the content of the zip file to the _CronfigBundle_ folder. `unzip -j cronfig.zip -d CronfigBundle`

1. [Download](https://cronfig.mautic.net/asset/1:mautic-cronfig-plugin) the plugin to your computer.
2. Upload and unzip. There are 2 ways to do it.
    2.1. If you have **SSH access** to your server:
    3.Unzip the downloaded package.
3. Upload the unzipped folder to the plugins folder and rename it to CronfigBundle the way you could locate CronfigBundle.php file on this path: plugins/CronfigBundle/CronfigBundle.php.
4. Clear Mautic's cache. Either run app/console cache:clear command in the Mautic's root dir or simply delete the content of app/cache dir.
5. Go to the right hand side Mautic menu (click the cog icon in the top right corner to slide the menu out) and go to Plugins.
6. Click the Install/Upgrade Plugins button. The Cronfig icon should appear in the list of plugins.
7. Go to the right hand side Mautic menu again. A new menu item called Cronfig should be there. Hit it. A register/login screen should appear.
8. Your email should be prefilled. Click on the Register button and check your email inbox. Your API key should appear in your inbox any second.
9. If you received the Cronfig registration email, copy the API key from it, insert it to the Log in input and log in.