# slack-darcula-css
Dark theme for Slack


<img src="https://raw.githubusercontent.com/mjacobsen4DFM/slack-darcula-css/master/Slack-Darcula.png" />

This is the original source of my CSS:<br/>
https://github.com/laCour/slack-night-mode/issues/73#issuecomment-287467332<br/>
It points to a publicly hosted CSS, which needs an ajax call appended to a Slack JS file.<br/>
<br/>
<br/>
But, I wanted to have it local so that I can edit and apply it, at will.<br/>
I saved it as /Applications/Resources/slack-darcula.css<br/>
<br/>
<br/>
Append this:
```
document.addEventListener('DOMContentLoaded', function() {
  var fs = require('fs'),
  filePath = '/Applications/Resources/slack-darcula.css';

  fs.readFile(filePath, {encoding: 'utf-8'}, function(err, data) {
    if (!err) {
      var css = document.createElement('style')
      css.innerText = data;
      document.getElementsByTagName('head')[0].appendChild(css);
    }
  })
});
```
to the appropriate interop file…<br/>
Mac:      /Applications/Slack.app/Contents/Resources/app.asar.unpacked/src/static/ssb-interop.js<br/>
Windows: %LocalAppData%\Slack<latest>\resources\app.asar.unpacked\src\static\ssb-interop.js<br/>
Ubuntu:  /usr/lib/slack/resources/app.asar.unpacked/src/static/ssb-interop.js<br/>
(I have only tested it on Mac)<br/> 
<br/>
CMD-R/CTRL-R will refresh the Slack window and apply the new CSS.<br/>
Nice and easy!<br/>
<br/>
All of the sidebar themes look okay, except Hoth.<br/>
I chose “Work Hard” for my sidebar theme.<br/>
<br/>
Ultimately, I customized it too. I was able to do it via the CSS; but the app lets you customize directly from preferences.<br/> 
These are my colors:<br/>
#545454,#ababab,#424242,#e6e6e6,#828282,#d8d8d8,#FFD700,#FFD700<br/>
<br/>
My eyes have thanked me!<br/>
(now, if only I could make *all* the white screens on my Mac dark!)<br/>
(Mojave says, "Hold my beer".)<br/>

