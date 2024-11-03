---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-10-30T18:08:16.998Z
updated: 2024-11-03T19:19:59.237Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/3f22ae9e837b10e05053cf12480b5c15e8d166c20b49b11db4fda3e3ee1b2757.jpg
---

## How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide

Viewing 6 posts - 1 through 6 (of 6 total)

* Author  
Posts
* February 12, 2012 at 2:15 pm [#10011](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/9dac5ab27354edc3ff070db8ce1a1a66?s=80&d=identicon&r=g)ToadLoadin](https://www.emeditor.com/forums/users/ToadLoadin/ "View ToadLoadin's profile")  
Member  
Hi, I’m writing some little AHK scripts to help my daily work, so I’m tweaking around the ahk syntax highlight configs.  
 Since I want to highlight subroutine labels of ahk script, I tried this pattern:  
^s*w+:(?=s*$|s*;.*$)  
 Which means words and a colon follows some space or right at the beginning of the line.  
 The “(?=s\*$|s\*;.\*$)” part is a [positive lookahead search](https://tools.techidaily.com/emeditor/products/), which means I want to have it could be followed by spaces or a line comment (; blah blah…), but it does not work as I expected, it can only be followed by spaces, once there is some comment followed, the highlight goes off.  
 Could anybody give me some hints how to correct it? :-)  
![](http://dl.dropbox.com/u/2516823/picture/2012-02/emeditor-syntax-highlight-with-regex-ahk-config.png)  
![](http://dl.dropbox.com/u/2516823/picture/2012-02/emeditor-syntax-highlight-with-regex.png)  
February 12, 2012 at 9:44 pm [#10012](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
 Don’t know. Seems to work for me.  
 EmEditor 11.0.5, 32-bit, Boost 1.47  
 What’s the differences?  
![](http://forentmp.lima-city.de/EmEditor_HighLight_RegEx_c16.png)  
February 13, 2012 at 5:16 am [#10013](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/9dac5ab27354edc3ff070db8ce1a1a66?s=80&d=identicon&r=g)ToadLoadin](https://www.emeditor.com/forums/users/ToadLoadin/ "View ToadLoadin's profile")  
Member  
囧 Quite weired…  
 I have exactly the same version.  
![](http://dl.dropbox.com/u/2516823/picture/2012-02/emeditor-1105-about.png)  
![](http://dl.dropbox.com/u/2516823/picture/2012-02/emeditor-1105-syntax-hightlithg-with-regex.png)  
February 13, 2012 at 5:19 am [#10014](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/9dac5ab27354edc3ff070db8ce1a1a66?s=80&d=identicon&r=g)ToadLoadin](https://www.emeditor.com/forums/users/ToadLoadin/ "View ToadLoadin's profile")  
Member  
EmEditor v11.0.5 (32bit)  
 under Win7 32bit, simplified Chinese…  
February 13, 2012 at 2:12 pm [#10016](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/9dac5ab27354edc3ff070db8ce1a1a66?s=80&d=identicon&r=g)ToadLoadin](https://www.emeditor.com/forums/users/ToadLoadin/ "View ToadLoadin's profile")  
Member  
Well, I got it.  
 It’s because there is a line comment setting which starts with the character “;”.  
 While the line comment setting turns off, the regex highlight works fine.  
 Hi Yutaka, is this a bug?  
February 13, 2012 at 6:23 pm [#10017](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hi ToadLoadin,  
 Currently, this is the specification. If the Line Comment character appear in the middle of a line, then the highlight will be turn off. This is because of optimization.  
 Thank you,
* Author  
Posts

Viewing 6 posts - 1 through 6 (of 6 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://instagram-videos.techidaily.com/updated-maximize-impact-mastering-igtv-content-submission-for-2024/"><u>[Updated] Maximize Impact Mastering IGTV Content Submission for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/2024-approved-easyrecorder-pro-free-gamers-recording-aid/"><u>2024 Approved EasyRecorder Pro Free Gamers' Recording Aid</u></a></li>
<li><a href="https://howto.techidaily.com/9-solutions-to-fix-vivo-v29-pro-system-crash-issue-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>9 Solutions to Fix Vivo V29 Pro System Crash Issue | Dr.fone</u></a></li>
<li><a href="https://techtrends.techidaily.com/compatibility-guide-using-airpods-with-the-nintendo-switch/"><u>Compatibility Guide: Using AirPods with the Nintendo Switch</u></a></li>
<li><a href="https://win-webster.techidaily.com/desole-windows-10-ne-demarre-pas-decouvrez-les-5-solutions-efficaces/"><u>Désolé, Windows 10 Ne Démarre Pas : Découvrez Les 5 Solutions Efficaces</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/exclusive-guide-turning-fb-videos-into-mp4-and-hd/"><u>Exclusive Guide Turning FB Videos Into MP4 & HD</u></a></li>
<li><a href="https://fox-http.techidaily.com/in-2024-enthralling-type-mobility-setups/"><u>In 2024, Enthralling Type Mobility Setups</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-use-allshare-cast-to-turn-on-screen-mirroring-on-xiaomi-redmi-a2plus-drfone-by-drfone-android/"><u>In 2024, How To Use Allshare Cast To Turn On Screen Mirroring On Xiaomi Redmi A2+ | Dr.fone</u></a></li>
<li><a href="https://win-webster.techidaily.com/page-missing-internet-search-yields-no-results-error-404/"><u>Page Missing – Internet Search Yields No Results (Error 404)</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/pinnacle-headlines-engineer-for-2024/"><u>Pinnacle Headlines Engineer for 2024</u></a></li>
<li><a href="https://common-error.techidaily.com/quick-solutions-resolving-unrecognized-usb-flash-drives/"><u>Quick Solutions: Resolving Unrecognized USB Flash Drives</u></a></li>
<li><a href="https://win-webster.techidaily.com/techniques-pour-recuperer-des-donnees-supprimees-dune-cle-usb-manuellement/"><u>Techniques Pour Récupérer Des Données Supprimées D'une Clé USB Manuellement</u></a></li>
<li><a href="https://win-webster.techidaily.com/top-ranking-windows-11-transfer-utility-seamless-movement-of-all-your-data/"><u>Top-Ranking Windows 11 Transfer Utility: Seamless Movement of All Your Data</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135351/19272" target="_top" id="2135351">
  <img src="//a.impactradius-go.com/display-ad/19272-2135351" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135351/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

