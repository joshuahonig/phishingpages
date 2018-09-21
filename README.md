# Phishing Pages
These pages can be customized to test how susceptible your staff are falling for a spear phishing campaign. Each folder contains specific information pertaining to that page. Please only use this for good.

# Important Note
Please use HTTPS on your phishing site. Nobody's credentials should be sent over the internet or over the local network in plain text. If you're not sure how to set that up, you can either use Cloudflare's free SSL, or EFF's [Certbot utility](https://certbot.eff.org/) to get yourself up and running with a free Let's Encrypt certificate.

# "It's not working!"
Are some elements of your page not loading? You may have mixed content. If you are running your site over HTTPS, make sure that the URLs for the elements on the page start with "https://".

Is Firefox complaining about your page? Make that if you site is running over HTTPS (it should be!), the link to the submission URL begings with "https://".

Make sure you test it in multiple browsers (yes, including Internet Explorer & Edge if the organization uses Windows), to make sure that it renders correctly.

# How should I store credentials?
[Curtis Brazzell's Phishing API](https://github.com/curtbraz/Phishing-API) is a wonderful project for just that! Most of these pages are designed to use it. 
