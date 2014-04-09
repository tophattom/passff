passff
======

[zx2c4 pass](http://www.zx2c4.com/projects/password-store/) manager addon for firefox


### Overview
This plugin will allow you to access your [pass](http://www.zx2c4.com/projects/password-store/) repository directly from firefox.

It will try to auto fill and auto submit the login form if a matching password entry is found

### Installation
- You have to have pass installed on your computer
- You will also need a working password repository
- Download the last release of the plugin [here](https://github.com/jvenant/passff/releases).
- You can then manually install the plugin in Firefox from the addons page (Firefox/Add-ons/Install Add-on from File...)

### Usage
A black icon with a P should appear in your Firefox toolbar.
From here, you will be able to browse your password repository.
Current supported features are :
- Fill and submit
- Goto, fill and submit
- Copy login to clipboard
- Copy password to clipboard

Additionnally, if you added an url property in your password info you will be able to go there clicking directly on the password menu (left-click same tab, middle-click new tab)

the accepted format for the password info is :  
&lt;the_password&gt;  
login: &lt;the_login&gt;  
url: &lt;the_url&gt;  

from the plugin preferences you will be able to set :
- A comma separated list of password input names. Input field names in a html page containing one of those values will be filled with the password
- A comma separated list of login input names. Input field names in a html page containing one of those values will be filled with the login
- A comma separated list of login field names. The first matching field in the password data will be used as login
- The pass script path
- Pass home. If empty, use User home
- Location of the gpg agent info file containing environment variables (relative to the home)


### The keyboard addicts like me will be happy
I **add a new button** displaying password repository in a list instead of a tree.
**This button will not be added automatically** to your Navigation toolbar.
You have to add it manually using the Customize menu (Right-click/Customize...) of the Navigation toolbar
This list has a shortcut : **Ctrl-y**
And a case sensitive **Fuzzy matching** algorithm.
So considering this repository
* Internet
 * MySite1
 * MySite2
* CoolStuf
  * SuperSite1
  * SuperSite2

&lt;Ctrl-y&gt;M1&lt;Enter&gt; will send you and authenticate you on MySite1 (&lt;Shift-Enter&gt; to open in a new tab)

This is a beta. For test purpose only
=========




