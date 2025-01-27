---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2025-01-24T23:55:06.367Z
updated: 2025-01-27T07:25:13.824Z
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
<li><a href="https://youtube-webster.techidaily.com/024-approved-free-audio-treasures-to-amplify-youtube/"><u>[New] 2024 Approved Free Audio Treasures to Amplify YouTube!</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ehind-the-camera-glory-spotlight-on-top-10-female-youtubers/"><u>[New] Behind-the-Camera Glory Spotlight on Top 10 Female YouTubers</u></a></li>
<li><a href="https://win-webster.techidaily.com/1-steps-to-monitor-your-printers-ink-supply-a-guide-by-yl-computing/"><u>1. Steps to Monitor Your Printer's Ink Supply: A Guide by YL Computing</u></a></li>
<li><a href="https://win-webster.techidaily.com/1732513921365-yl-software/"><u>在武则天的时代，有多少政令违背其初心？ YL Software的专业解构</u></a></li>
<li><a href="https://win-webster.techidaily.com/elegant-gold-digital-artwork-for-screens-professional-image-collection-from-yl-software/"><u>Elegant Gold Digital Artwork for Screens: Professional Image Collection From YL Software</u></a></li>
<li><a href="https://youtube-web.techidaily.com/24-the-chronicles-uncovered-top-10-historians-youtube-picks/"><u>In 2024, The Chronicles Uncovered Top 10 Historian's YouTube Picks</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-the-easy-way-to-remove-an-apple-id-from-your-macbook-for-your-iphone-xr-by-drfone-ios/"><u>In 2024, The Easy Way to Remove an Apple ID from Your MacBook For your iPhone XR</u></a></li>
<li><a href="https://win-excellent.techidaily.com/step-by-step-tutorial-setting-up-vcenter-server-appliance-with-esxi/"><u>Step-by-Step Tutorial: Setting Up vCenter Server Appliance with ESXi</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/swap-and-sync-connecting-your-logitech-wireless-mouse-to-another-transmitter/"><u>Swap and Sync: Connecting Your Logitech Wireless Mouse to Another Transmitter</u></a></li>
<li><a href="https://hardware-help.techidaily.com/1722965824999-the-seat-of-arbitration-determines-the-procedural-law-that-governs-the-arbitration-process-and-can-affect-the-degree-of-court-intervention/"><u>The Seat of Arbitration Determines the Procedural Law that Governs the Arbitration Process and Can Affect the Degree of Court Intervention.</u></a></li>
<li><a href="https://win-webster.techidaily.com/the-ultimate-recovery-solution-retrieving-permanently-deleted-files-in-windows-environments-with-yl-software-support/"><u>The Ultimate Recovery Solution: Retrieving Permanently Deleted Files in Windows Environments with YL Software Support</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/tips-for-a-seamless-experience-accessing-youtube-video-comments/"><u>Tips for a Seamless Experience Accessing YouTube Video Comments</u></a></li>
<li><a href="https://win-webster.techidaily.com/unlock-greater-sound-quality-expert-guide-to-boosting-your-sound-cards-performance-with-yl-software-solutions/"><u>Unlock Greater Sound Quality: Expert Guide to Boosting Your Sound Card's Performance with YL Software Solutions</u></a></li>
<li><a href="https://win-webster.techidaily.com/unveiling-hidden-threats-how-to-identify-viruses-and-malware-in-your-computer-system-tips-from-yl-software-experts/"><u>Unveiling Hidden Threats: How to Identify Viruses & Malware in Your Computer System - Tips From YL Software Experts</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/SgRVYjqB70s?si=My_2cDvJVdincQRu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

