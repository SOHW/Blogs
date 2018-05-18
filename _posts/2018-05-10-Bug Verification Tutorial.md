---
layout: post

#event information
title:  "Bug Verification Day Tutorial"
description: "To add resources.."
cover: "assets/images/qa/qmo.jpg "
comments: true

#event organiser details
author: "Surentharan"
category: "Quality Assurance"

---

Welcome to Bug Verification Day !!!

<b>Step 1:</b><br>
&nbsp;&nbsp; Go to [Bugzilla](http://bugzilla.mozilla.org/) website and sign in your account if you already have a account , else create a new one.<br>

  ![bugzilla main page sign in]({{ site.url }}/assets/images/qa/bugzilla main page sign in.jpg)<br>
  
<b>Step 2:</b><br>
<ol>
  <li>In order to confirm bugs, you need the "canconfirm" privilege.</li>
  <li>If you've been active in Bugzilla, you may already have this [privilege](https://bugzilla.mozilla.org/userprefs.cgi?tab=permissions). Check your Bugzilla preferences. If your Permissions include "Can confirm a bug", then you are all set.</li>
  <li>If not, want to have canconfirm permission, you can add it yourself using the [triage request form](https://bugzilla.mozilla.org/page.cgi?id=triage_request.html)</li>
</ol>

<b>Step 3:</b><br>
&nbsp;&nbsp; Open the etherpad (the etherpad link can be found in the [telegram group](https://t.me/MozIndia_QA) ) and enter your details such as name, OS along with 32 or 64 bit.
<ul>
  <li>Don't forget to add your name at the top of the etherpad and choose your color.</li>
  <li>Please don't overwrite others content</li>
</ul>
  
<b>Step 4:</b><br>
&nbsp;&nbsp; Update your browser or you can download the browser from the link provided in the etherpad. If you update the browser please check the browser version with the browser version mentioned in the etherpad.
<ul>
  <li>Please make sure that you are using the latest version , if not update or download from the link given in the etherpad.</li>
</ul>

<b>Step 5:</b><br>
&nbsp;&nbsp; Open the list of bugs to verify. While opening the list of bugs choose the link for the browser which you are currently working.
For example: If I am working with nightly I have to open the bug list for nightly browser.



<b>Step 6 :</b></br>
&nbsp;&nbsp; Choose a bug from the list

<b>Step 7:</b><br> 
After choosing the bug :  
First verify whether the bug is marked as Resolved and Fixed.
Take note of the platforms / operating systems affected by the bug.
Read all the comments in order to understand the bug.
Download an affected build and reproduce the issue.
Download latest Firefox builds, on which the bug has been fixed and try to reproduce the bug again.
Try to also test around the fixed area, to make sure nothing got broken when the bug has been fixed.
Step 8:
Scenarios you might encounter:
If unable to understand the issue, ask for more information..
If the issue can't be reproduced by the tester, a comment must be added asking for more information or just notifying that the issue could not  be reproduced. In this case is not relevant verifying the bug on latest builds.
If the issue is reproducible only on a specific platform at which the tester don't have access too, then verifying the issue is also not relevant.
If better STR are provided in the comments below comment0, then those STR must be used in order to verify the bug.
If the build with the fix is not released, we use tinderbox builds, or wait until the build is available.
If another issue is found while verifying a bug, we check to see if the issue is not already logged and if not, log a new bug.

For example :
I have chosen this bug https://bugzilla.mozilla.org/show_bug.cgi?id=1300376




After doing the steps mentioned in Step 7, I clearly understood what the bug is and reproduced the bug and found the bug has been fixed. If you can't understand the bug then u can refer step 8
While reproducing the bug if you find the bug has not been fixed then u can mention it the comment

<b>Step 9:</b><br>At the top click edit option



Step 10 : 
[If you could not reproduce the bug or not sure if its verified, please ignore this step]    
Under tracking flag section , you can see a list of option corresponding to their respective browsers (refer screenshot below) 



Select verified from the drop down list of the browser in which you have reproduced the bug.( In this case Firefox 55)

Step 11:
           Comment in detail about the status of the bug ,the system and browser configuration you're working on. You can also add screenshots describing the bugs if necessary . While commenting don't forget to add [bugday-yyyymmdd] .
If in need of any further information about the bug , check the Need more information from check box.



 Step 12: Proceed with Save Changes.

 Step 13: Paste the bug URL in the etherpad.




Note :
Before verifying the bug ... try to find the affected build .  U can find them in the comment section of the bug .
Download the affected build from [ https://archive.mozilla.org/pub/firefox/ ] and verify whether you can reproduce the bug . If you can reproduce the bug in the affected build then proceed with verifying the bugs in the latest build . If you cannot reproduce the bug then no need to verify the bug in the latest build . Comment the bug details briefly ....

If you have any doubts feel free to ask in this Telegram group or IRC chat. If you have any queries regarding this blog please contact me using Telegram or email me at [ surentharan14@gmail.com ]

<center><b><h1>Happy Bug Verification Day!</h1></b></center>
