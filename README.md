psdle
=====

Improving everyone's favorite online download list, one loop at a time.

Doubtful? Have some in-action screenshots:    
[PS4 games](http://i.imgur.com/hFIw450.png) Example: All Plus offerings.    
[PS3 games, no unlocks or passes](http://i.imgur.com/1Iz43kd.png) Example: DS3 has an online pass, DDU has an unlock.    
[PS3+V games](http://i.imgur.com/WekNUVc.png) Example: Plus offerings for PS3+V.

Usage
=====
1. Navigate to the desired account's download page from the online store
2. Ensure the displayed page is the first (top has latest purchase)
3. Open either the browser's Scratchpad (Shift+F4) or Web Console (Ctrl+Shift+K) (Firefox)
4. Input **$.getScript("https://raw.githubusercontent.com/RePod/psdle/master/psdle.js");**
5. Execute (Ctrl+R in Scratchpad, Enter in Console) and let the magic happen

What Needs To Be Done
=====
* In-depth information gathering (i.e. if system filtering is vague such as PS1 games marked for PSP)

Potentially Asked Questions
=====
###Why does it take so long to parse?
PSDLE works by parsing each page of the download list one at a time with a delay inbetween. Currently a timeout of 3 seconds seems to hit the sweet spot of changing the page and detecting the content (on a reasonable connection and assuming the server isn't already dying).
This may change in the future.

###Why are thumbnails/icons missing?
Seems to be a cache issue, a noticable solution would be going to problematic pages then running PSDLE again.    
Trust me, I noticed.

###Why is this so horrible?
At the time of writing a concept version is available simply showing off what can be done.    
Feel free to fork and submit pull requests.

###Why is this so good?
I ask myself that every time I wake up.

###Does this work in any browser/my toaster's web browser?
Probably, as long as it allows local Javascript execution.

###Is this safe or a ploy to phish account details?
I put it on GitHub for a reason, feel free to view the ~~horribly effective~~ code yourself and decide.    
If and when I get pull requests I'll let them sizzle and look through them while allowing the "community" to as well.

If authentication details were left around openly on the download list page I would take my concerns elsewhere.