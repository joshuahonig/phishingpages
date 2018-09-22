# Secure Document
The idea of this page is to have the user enter their credentials under the pretense of viewing a "secure document", and execute a malicious document. The user can then either redirected to a fake error page so as not to raise suspicion (error.html), or be redirected to a document download page (download.html).
It is designed to be used with [Curtis Brazzell's Phishing API](https://github.com/curtbraz/Phishing-API). 
![Landing Page Image](https://i.imgur.com/BSZ6YbW.jpg)
![Download Page Image](https://i.imgur.com/XeoH40U.jpg)
![Error Page Image](https://i.imgur.com/1RVAknx.jpg)

#### The following sections specify which lines should be customized. 
# index.html
---
index.html:
Line 16- Change the organization name.
Line 23- Change the URL to submit to. 
Line 24- Change the path to the image, and tinker with the image width to make it look right. The seal of the state of Indiana has been used as an example.
Lines 26- Change the wording of this text to more properly suit the organization.
Lines 27, 28- Change `rgb(4, 14, 99)` to something else if you'd like the text boxes to have a different outline color. 
Line 29- Change the project ID. See the page on Curtis Brazzell's Phishing API for more information. 
Lines 30- Change the redirect page to error.html if you wish to use it. See the page on Curtis Brazzell's Phishing API for more information. 
# style.css
---
Lines 92 thru 96- Change the background color. It's not a bad idea to have this match the color of your organization's logo, if applicable. 
# error.html
---
Line 5- Change the organization name. 
Lines 14- The JavaScript that is run on button click can be modified. 
# download.html
---
Line 5- Change the organization name. 
Lines 14- Change the `href` to contain the URL to your document. 
# Other notes & tips
---
favicon.ico- The website's icon, if this folder is at the web root (browsers should be able to load this at  {your site}/favicon.ico).
emblem.png- The image shown on the login page. See line 24 of index.html.
To make the URL more believable and lower suspicion, it may not be a bad idea to have it end with a fake document ID. For example:
`https://badsite.com/?documentid=hvhB8dVRhhX1HDiUcCqD`