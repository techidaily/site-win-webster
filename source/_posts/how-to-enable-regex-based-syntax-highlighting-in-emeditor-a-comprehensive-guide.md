---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-11-28T01:51:38.162Z
updated: 2024-12-01T00:40:54.841Z
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
<li><a href="https://fox-access.techidaily.com/new-inside-the-directors-suite-powerdirector-2024-deep-dive/"><u>[New] Inside the Director's Suite PowerDirector 2024 Deep Dive</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gourmet-visuals-in-motion-food-shot-tips-and-tricks/"><u>[Updated] Gourmet Visuals in Motion Food Shot Tips & Tricks</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-in-2024-dji-aerial-innovation-packs-starter-pro-upgrade-high-definition-ultra/"><u>[Updated] In 2024, DJI Aerial Innovation Packs Starter, Pro Upgrade, High-Definition Ultra</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-in-2024-perfecting-picture-in-picture-setup-with-youtube-on-ios/"><u>[Updated] In 2024, Perfecting Picture-in-Picture Setup with YouTube on iOS</u></a></li>
<li><a href="https://extra-support.techidaily.com/updated-mastering-pubg-tones-in-minutes/"><u>[Updated] Mastering PUBG Tones in Minutes</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-mastering-the-airwaves-dji-drones-and-social-media-live/"><u>[Updated] Mastering the Airwaves DJI Drones and Social Media Live</u></a></li>
<li><a href="https://win-webster.techidaily.com/aomei-image-deploy-wie-man-ein-bild-bereitstellt-wenn-keine-sid-vorhanden-ist/"><u>AOMEI Image Deploy: Wie Man Ein Bild Bereitstellt, Wenn Keine SID Vorhanden Ist</u></a></li>
<li><a href="https://win-webster.techidaily.com/herstellung-einer-versteckten-wiederherstellungspartition-fur-windows-7-schritt-fur-schritt-anleitung/"><u>Herstellung Einer Versteckten Wiederherstellungspartition Für Windows 7: Schritt-Für-Schritt-Anleitung</u></a></li>
<li><a href="https://unlock-android.techidaily.com/how-to-unlock-honor-90-pro-phone-with-broken-screen-by-drfone-android/"><u>How to Unlock Honor 90 Pro Phone with Broken Screen</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/precision-editing-perfecting-the-art-of-fades-in-pro/"><u>Precision Editing Perfecting the Art of Fades in Pro</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ce-steps-how-to-turn-your-yt-queue-on-its-head-for-2024/"><u>Retrace Steps How to Turn Your YT Queue on Its Head for 2024</u></a></li>
<li><a href="https://win-webster.techidaily.com/seamless-install-von-windows-11-auf-nicht-zertifizierten-geraten-sichere-methode-ohne-datenverlust/"><u>Seamless Install Von Windows 11 Auf Nicht-Zertifizierten Geräten - Sichere Methode Ohne Datenverlust</u></a></li>
<li><a href="https://win-webster.techidaily.com/step-by-step-tutorial-on-copying-music-from-itunes-to-iphone-iphone-151413-by-bypassing-traditional-synchronization/"><u>Step-by-Step Tutorial on Copying Music From iTunes to iPhone (iPhone 15/14/13) by Bypassing Traditional Synchronization</u></a></li>
<li><a href="https://win-webster.techidaily.com/the-ultimate-walkthrough-building-flawless-windows-disk-images-using-leading-free-software/"><u>The Ultimate Walkthrough: Building Flawless Windows Disk Images Using Leading Free Software</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/xg3PHS_Ee80?si=fE_iGIqHjKvWFIN3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

