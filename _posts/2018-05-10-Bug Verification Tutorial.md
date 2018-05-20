---
layout: post

#event information
title:  "Bug Verification Tutorial"
description: "To add resources.."
cover: "assets/images/qa/qmo.jpg "
comments: true

#event organiser details
author: "Surentharan"
category: "Quality Assurance"

---

## Welcome!!!

### Step 1:

Navigate to [Bugzilla](http://bugzilla.mozilla.org/) website and sign in your account if you already have a account, else create a new one.
   
{% include image.html url="https://3.bp.blogspot.com/-cnyX57F07ZA/WPdgy2AbZAI/AAAAAAAAAlA/py1Wxq9CASosXmycvafoGwGIf3TTeSJWwCLcB/s640/bugzilla%2Bmain%2Bpage%2Bsign%2Bin.jpg" width="100%" description="" %}

  
### Step 2:
* In order to confirm bugs, you need the **canconfirm** privilege
* If you've been active in Bugzilla, you may already have this [privilege](https://bugzilla.mozilla.org/userprefs.cgi?tab=permissions). Check your Bugzilla preferences. If your Permissions include "Can confirm a bug", then you are all set.</li>
* If not, want to have canconfirm permission, you can add it yourself using the [triage request form](https://bugzilla.mozilla.org/page.cgi?id=triage_request.html)

### Step 3:

Open the etherpad (the etherpad link can be found in the [telegram group](https://t.me/MozIndia_QA)) and enter your details such as name, OS along with 32 or 64 bit.

  * Don't forget to add your name at the top of the etherpad and choose your color
  * Please don't overwrite others content
  
{% include image.html url="https://2.bp.blogspot.com/-xSqbKR91CY4/WPdpsJKERBI/AAAAAAAAAl0/W-bTa63I0Wkls7VlOEWsHTZZFI3Tp99_QCLcB/s640/etherpad.jpg" width="100%" description="" %}

  
### Step 4:

Update your browser or you can download the browser from the link provided in the etherpad. If you update the browser please check the browser version with the browser version mentioned in the etherpad.

* Please make sure that you are using the latest version , if not update or download from the link given in the etherpad

{% include image.html url="https://2.bp.blogspot.com/-HWgEDZPwRz0/WPykUAYumgI/AAAAAAAAAps/FHCIw_--8h4N6rgn9q3BkRj86iqWnp15ACEw/s640/1.jpg" width="100%" description="" %}

{% include image.html url="https://1.bp.blogspot.com/--xSW5xciPzc/WPykVBgO18I/AAAAAAAAAps/bLZVvoUTirwiIzSOLFmYOiHOQ41G76fAQCEw/s640/2.jpg" width="100%" description="" %}

{% include image.html url="https://4.bp.blogspot.com/-UP3mQ-U_mI4/WPykSzBfC_I/AAAAAAAAAps/3-pMhMQcBsMgdWvLaqXSI_9czIGJwyLogCEw/s640/3.jpg" width="100%" description="" %}

{% include image.html url="https://1.bp.blogspot.com/-1QEiJWS0co0/WPykXBK9zuI/AAAAAAAAAps/haW0khpUgY4vyAKRLyOv8B0FvGpyNxY_gCEw/s640/4.jpg" width="100%" description="" %}

### Step 5:

Open the list of bugs to verify. While opening the list of bugs choose the link for the browser which you are currently working.

*For example: If I am working with nightly I have to open the bug list for nightly browser.*

{% include image.html url="https://3.bp.blogspot.com/-9ET7LEbga-4/WPds0JF37eI/AAAAAAAAAmA/bc278Fw5tc4nxSFCjWgL3_kGmPM4-agZgCLcB/s640/etherpad%2B1.jpg" width="100%" description="" %}


### Step 6:

Choose a bug from the list

### Step 7:

After choosing a bug:
* First verify whether the bug is marked as Resolved and Fixed
* Take note of the platforms / operating systems affected by the bug
* Read all the comments in order to understand the bug
* Download an affected build and reproduce the issue
* Download latest Firefox builds, on which the bug has been fixed and try to reproduce the bug again
* Try to also test around the fixed area, to make sure nothing got broken when the bug has been fixed


### Step 8:
Scenarios you might encounter:
* If unable to understand the issue, ask for more information
* If the issue can't be reproduced by the tester, a comment must be added asking for more information or just notifying that the issue could not  be reproduced. In this case is not relevant verifying the bug on latest builds
* If the issue is reproducible only on a specific platform at which the tester don't have access too, then verifying the issue is also not relevant
* If better STR are provided in the comments below comment0, then those STR must be used in order to verify the bug
* If the build with the fix is not released, we use tinderbox builds, or wait until the build is available
* If another issue is found while verifying a bug, we check to see if the issue is not already logged and if not, log a new bug

*For example :
I have chosen this bug [https://bugzilla.mozilla.org/show_bug.cgi?id=1300376](https://bugzilla.mozilla.org/show_bug.cgi?id=1300376)
  
{% include image.html url="https://2.bp.blogspot.com/-YX6TwRAmU48/WPd3QRyZ8oI/AAAAAAAAAm0/-zGMaTiAk5QWYDuA3pl5Ycw7xd9qmkq4QCLcB/s640/1.jpg" width="100%" description="" %}

After doing the steps mentioned in **Step 7**, I clearly understood what the bug is and reproduced the bug and found the bug has been fixed. If you can't understand the bug then u can refer **step 8**.
While reproducing the bug if you find the bug has not been fixed then u can mention it the comment

### Step 9:

At the top click edit option

{% include image.html url="https://2.bp.blogspot.com/-V_zgwSa-1_w/WPd4xVrwA4I/AAAAAAAAAnM/xD-y4kHy59Q15pexqTlwqu21UoNrYECeQCLcB/s640/2.jpg" width="100%" description="" %}

### Step 10 :
*[If you could not reproduce the bug or not sure if its verified, please ignore this step]*    
Under tracking flag section , you can see a list of option corresponding to their respective browsers (refer screenshot below) 

{% include image.html url="https://1.bp.blogspot.com/-lGf5i1zM9yE/WPd6hT6_4qI/AAAAAAAAAnk/1TSXDfh1czsCaet20uvbp6yci1aAtJFeACLcB/s640/3.jpg" width="100%" description="" %}

Select `verified` from the drop down list of the browser in which you have reproduced the bug. (In this case Firefox 55)

### Step 11:
* Comment in detail about the status of the bug, the system and browser configuration you're working on. You can also add screenshots describing the bugs if necessary 
* While commenting don't forget to add **[bugday-yyyymmdd]** specified in the respective etherpad
* If in need of any further information about the bug , check the `*Need more information*` from check box and ask the information that you are looking for

{% include image.html url="https://2.bp.blogspot.com/-Q9DCrAGy68Y/WPeDUzFoKZI/AAAAAAAAAoM/RsOXz4RWPcsocA743gPqkNGBhuxe20t4QCLcB/s640/4.jpg" width="100%" description="" %}


### Step 12:
Proceed with `Save Changes`

### Step 13:
Paste the bug URL in the etherpad

{% include image.html url="https://3.bp.blogspot.com/-_ofyByp5Vac/WPeHHUdseyI/AAAAAAAAAow/--JA0hEFsg8AFr9U2KiVje5Nx1umk34ZgCLcB/s640/final%2Betherpad.jpg" width="100%" description="" %}




~~~
#### Note: 
* Before verifying the bug, try to find the affected build. You can find them in the comment section of the bug.
* Download the affected build from [https://archive.mozilla.org/pub/firefox/](https://archive.mozilla.org/pub/firefox/) and verify whether you can reproduce the bug. 
* If you can reproduce the bug in the affected build then proceed with verifying the bugs in the latest build. If you cannot reproduce the bug then no need to verify the bug in the latest build. 
* Comment the bug details briefly ....

~~~

If you have any doubts feel free to ask in this [Telegram group](https://t.me/MozIndia_QA) or [IRC chat](http://widget01.mibbit.com/?server=irc.mozilla.org&channel=%23qa). If you have any queries regarding this blog please contact me using [Telegram](https://t.me/surenvino) or email me at [surentharan14@gmail.com]

<center><b><h1>Happy Bug Verification!</h1></b></center>
