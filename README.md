# slack-darcula-css
Dark theme for Slack


<img src="https://raw.githubusercontent.com/mjacobsen4DFM/slack-darcula-css/master/Slack-Darcula.png" />

This is the original source of my CSS:<br/>
https://github.com/laCour/slack-night-mode/issues/73#issuecomment-287467332<br/>
It points to a publicly hosted CSS, which needs an ajax call appended to a Slack JS file.<br/>
<br/>
<br/>
But, I wanted to have it local so that I can edit and apply it, at will.<br/>

Now, you can too!
<br/>
Save the css as /Applications/Resources/slack-darcula.css<br/>
<br/>
Run slack4-darcula-mode.bsh
It will unpack Salck, alter /app.asar.unpacked/dist/ssb-interop.bundle.js to load ths CSS, and repack Slack.
<br/> 
(Note: I have only tested it on Mac)<br/> 
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

/////
Special thanks to @d-fay for the unpack/pack script!
