---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-11-16T00:32:00.526Z
updated: 2024-11-22T18:33:10.074Z
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
<li><a href="https://video-screen-grab.techidaily.com/new-achieving-perfect-pitch-captures-in-rl-games/"><u>[New] Achieving Perfect Pitch Captures in RL Games</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-2024-approved-360-camera-buying-guide-how-to-choose-a-suitable-360-camera/"><u>[Updated] 2024 Approved 360 Camera Buying Guide How to Choose a Suitable 360 Camera</u></a></li>
<li><a href="https://some-guidance.techidaily.com/updated-unleash-your-videos-potential-thriving-in-youtube-rankings/"><u>[Updated] Unleash Your Video's Potential Thriving in YouTube Rankings</u></a></li>
<li><a href="https://win-webster.techidaily.com/windows7810backup4all/"><u>安心と利便性を融合: Windows7、8、10に適した無料強力バックアップツールでBackup4allを超える</u></a></li>
<li><a href="https://win-webster.techidaily.com/beat-the-frustration-essential-strategies-for-handling-cannot-open-file-corrupted-issues/"><u>Beat the Frustration: Essential Strategies for Handling 'Cannot Open - File Corrupted' Issues</u></a></li>
<li><a href="https://win-webster.techidaily.com/correzione-dellimmagine-di-ripristino-sistema-eccezionale-a-causa-di-problemi-biosefi/"><u>Correzione Dell'Immagine Di Ripristino Sistema Eccezionale a Causa Di Problemi BIOS/EFI</u></a></li>
<li><a href="https://win-webster.techidaily.com/directly-setting-up-windows/"><u>Directly Setting Up Windows</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/o-use-youtube-enhancements/"><u>How to Use YouTube Enhancements</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-transform-ordinary-moments-into-extraordinary-art-creating-slow-motion-video-from-still-images-online/"><u>In 2024, Transform Ordinary Moments Into Extraordinary Art Creating Slow Motion Video From Still Images Online</u></a></li>
<li><a href="https://buynow-info.techidaily.com/in-depth-review-amazing-versatility-with-amazonbasics-7-port-usb-30-hub/"><u>In-Depth Review: Amazing Versatility with AmazonBasics 7-Port USB 3.0 Hub</u></a></li>
<li><a href="https://win-webster.techidaily.com/macrium-reflect-solved-successfully-unmounting-volumes-in-three-simple-methods/"><u>Macrium Reflect Solved: Successfully Unmounting Volumes in Three Simple Methods</u></a></li>
<li><a href="https://sound-issues.techidaily.com/stop-frustrating-cuts-in-discord-chat-master-audio-fixes-with-our-2ebsy-tips/"><u>Stop Frustrating Cuts in Discord Chat: Master Audio Fixes with Our 2Ebsy Tips</u></a></li>
<li><a href="https://tech-haven.techidaily.com/the-ultimate-tutorial-on-harnessing-chatgpt-capabilities-across-various-languages/"><u>The Ultimate Tutorial on Harnessing ChatGPT Capabilities Across Various Languages</u></a></li>
<li><a href="https://win-webster.techidaily.com/urutan-rasa-pilihan-ubah-gaya-memutakhirkan-file-lama-di-google-drive-selamat-tahun-baru/"><u>Urutan Rasa Pilihan: Ubah Gaya Memutakhirkan File Lama Di Google Drive Selamat Tahun Baru!</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9wiIVztRIqQ?si=GBgdwQ78k5hbeFDv&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

