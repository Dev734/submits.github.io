# Advanced Info Logger + URL Shortener

## Usage
To create a URL, format it like this:

submits.github.io/?*(user id of who you want to ping when url is clicked)*?*(id of webhook)*?*(token of webhook)*?*(message victim will see upon loading page)*

Optionally, add *?mobile* on the end of the url if you are targetting someone on mobile (this is because some info only supports desktop browsers).

Alternatively, you can go *[here](https://submits.github.io/create.html)* to easily create a link.

## Example URL:
https://submits.github.io/?111111111111111111?000000000000000000?5GQxDgWlCxxIgKqNiOedfzv-dKI_lE0qxq5R4ZiBDngj619JdLiHkH6N2FPB1Vl2qDIw?an%20example%20logging%20message?mobile

*It is recommended you use a URL shortener (My own custom one is linked [here](https://submits.github.io/shorten.html))*

## Result

![Clicking on the link should produce this from your webhook.](https://i.imgur.com/ch3F020.png)

The webhook name will be randomised to avoid clutter, the user mentioned in the URL will be pinged, and the embed will contain the following:<br>
• *The URL the victim clicked  <br>
• IP <br>
• Rough Area  <br>
• Postcode <br>
• Lat/Long of IP <br>
• Browser <br>
• Platform <br> 
• Screen Size <br>
• Screen Rotation (UNAVAILABLE FOR MOBILE) <br>
• Batter Percentage (UNAVAILABLE FOR MOBILE) <br>
• Graphics Card Name/Driver <br>
• Number of Logical Processors <br>
• The message the victim will see <br>*

## URL Shortener

The [URL shortener](https://submits.github.io/shorten.html) does not need to be used specifically for info logging, and is just a small extra thing I made that is still a work in progress

### How does it work?<br>
When you input a name and url, it sends it to a database which stores these two pieces of data together.  Whilst this is happening, it also checks the name used against every other domain in the database, and if it is the same as another domain it will reject the request to add it to the database. However, it is successful, the domain will be added and whenever you load the outputted url it will extract the url from the database based of the name parsed into the url and redirect you.

### Limitations<br>
The database software this currently uses can store around 50k urls a month, with 5GB of raw text requests able to be sent.
