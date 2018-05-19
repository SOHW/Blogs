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
<i>For example:</i> If I am working with nightly I have to open the bug list for nightly browser.



<b>Step 6 :</b></br>
&nbsp;&nbsp; Choose a bug from the list

<b>Step 7:</b><br> 
After choosing the bug :<br>
<ul>
  <li>First verify whether the bug is marked as Resolved and Fixed.</li>
  <li>Take note of the platforms / operating systems affected by the bug.</li>
  <li>Read all the comments in order to understand the bug.</li>
  <li>Download an affected build and reproduce the issue.</li>
  <li>Download latest Firefox builds, on which the bug has been fixed and try to reproduce the bug again.</li>
  <li>Try to also test around the fixed area, to make sure nothing got broken when the bug has been fixed.</li>
 </ul>
 <br> 
 
<b>Step 8:</b><br>
Scenarios you might encounter:<br>
<ul>
  <li>If unable to understand the issue, ask for more information..</li>
  <li>If the issue can't be reproduced by the tester, a comment must be added asking for more information or just notifying that the issue could not  be reproduced. In this case is not relevant verifying the bug on latest builds.</li>
  <li>If the issue is reproducible only on a specific platform at which the tester don't have access too, then verifying the issue is also not relevant.</li>
  <li>If better STR are provided in the comments below comment0, then those STR must be used in order to verify the bug.</li>
  <li>If the build with the fix is not released, we use tinderbox builds, or wait until the build is available.</li>
  <li>If another issue is found while verifying a bug, we check to see if the issue is not already logged and if not, log a new bug.</li>
  </ul>
  <br>

<b><i>For example :<b></i><br>
&nbsp;&nbsp; I have chosen this bug [https://bugzilla.mozilla.org/show_bug.cgi?id=1300376](https://bugzilla.mozilla.org/show_bug.cgi?id=1300376)<br>
  

&nbsp;&nbsp; After doing the steps mentioned in Step 7, I clearly understood what the bug is and reproduced the bug and found the bug has been fixed. If you can't understand the bug then u can refer step 8<br>
While reproducing the bug if you find the bug has not been fixed then u can mention it the comment<br>

<b>Step 9:</b><br>At the top click edit option



<b>Step 10 :<p>[If you could not reproduce the bug or not sure if its verified, please ignore this step]</p></b><br>    
&nbsp;&nbsp; Under tracking flag section , you can see a list of option corresponding to their respective browsers (refer screenshot below) 



Select verified from the drop down list of the browser in which you have reproduced the bug.( In this case Firefox 55)

Step 11:
&nbsp;&nbsp; Comment in detail about the status of the bug ,the system and browser configuration you're working on. You can also add screenshots describing the bugs if necessary . While commenting don't forget to add <b><p>[bugday-yyyymmdd]</p></b>.<br>
If in need of any further information about the bug , check the <b>Need more information</b> from check box.<br>


<b>Step 12:</b> Proceed with <b>Save Changes.</b><br>

<b> Step 13:</b> Paste the bug URL in the etherpad.<br>




<b>Note :<br>
Before verifying the bug ... try to find the affected build .  U can find them in the comment section of the bug.<br>
Download the affected build from [https://archive.mozilla.org/pub/firefox/](https://archive.mozilla.org/pub/firefox/) and verify whether you can reproduce the bug . If you can reproduce the bug in the affected build then proceed with verifying the bugs in the latest build . If you cannot reproduce the bug then no need to verify the bug in the latest build . Comment the bug details briefly ....<b>

If you have any doubts feel free to ask in this [Telegram group](https://t.me/MozIndia_QA) or [IRC chat](http://widget01.mibbit.com/?server=irc.mozilla.org&channel=%23qa). If you have any queries regarding this blog please contact me using [Telegram](https://t.me/surenvino) or email me at <b>[surentharan14@gmail.com]</b><br><br>

<center><b><h1>Happy Bug Verification Day!</h1></b></center>
