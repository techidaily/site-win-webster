---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-11-10T21:24:23.968Z
updated: 2024-11-12T23:51:44.261Z
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
<li><a href="https://facebook-video-share.techidaily.com/new-enhance-engagement-top-12-tactics-for-youtube-success-for-2024/"><u>[New] Enhance Engagement Top 12 Tactics for YouTube Success for 2024</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-2024-approved-fixing-the-obs-fullscreen-hurdle/"><u>[Updated] 2024 Approved Fixing the OBS Fullscreen Hurdle</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-2024-approved-optimal-obs-configurations-for-thrifty-computers/"><u>[Updated] 2024 Approved Optimal OBS Configurations for Thrifty Computers</u></a></li>
<li><a href="https://article-files.techidaily.com/updated-stream-your-podcast-with-one-move-only/"><u>[Updated] Stream Your Podcast with One Move Only</u></a></li>
<li><a href="https://win-webster.techidaily.com/windows-cmdcmd/"><u>啟動Windows CMD課程：深入了解透過CMD處理檔案操作方法</u></a></li>
<li><a href="https://win-webster.techidaily.com/come-aumentare-la-durata-e-le-prestazioni-del-tuo-pc-sostituendo-lssd-xps-con-un-modello-di-capacita-maggiore/"><u>Come Aumentare La Durata E Le Prestazioni Del Tuo PC Sostituendo L'SSD XPS Con Un Modello Di Capacità Maggiore</u></a></li>
<li><a href="https://win-webster.techidaily.com/data-rescue-tactics-retrieving-information-from-a-faulty-flash-drive-without-erasing-contents/"><u>Data Rescue Tactics: Retrieving Information From a Faulty Flash Drive Without Erasing Contents</u></a></li>
<li><a href="https://win-webster.techidaily.com/detailed-tutorial-on-creating-and-configuring-networks-using-vmwares-vcenter-software/"><u>Detailed Tutorial on Creating and Configuring Networks Using VMware's vCenter Software</u></a></li>
<li><a href="https://win-solutions.techidaily.com/guia-passo-a-passo-para-gravar-videos-em-camera-lenta-no-android-usando-o-aplicativo-movavi-clips/"><u>Guia Passo a Passo Para Gravar Vídeos Em Câmera Lenta No Android Usando O Aplicativo Movavi Clips</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-watch-hulu-outside-us-on-realme-11-pro-drfone-by-drfone-virtual-android/"><u>How to Watch Hulu Outside US On Realme 11 Pro | Dr.fone</u></a></li>
<li><a href="https://win-webster.techidaily.com/how-to-article-generate-personalized-windows-11-installation-image-iso-file/"><u>How-To Article: Generate Personalized Windows 11 Installation Image (ISO) File</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-passfab-iphone-11-pro-backup-unlocker-top-4-alternatives-by-drfone-ios/"><u>In 2024, PassFab iPhone 11 Pro Backup Unlocker Top 4 Alternatives</u></a></li>
<li><a href="https://win-webster.techidaily.com/locating-the-timestamp-of-your-latest-iphone-icloud-sync-a-comprehensive-tutorial-for-users-and-administrators/"><u>Locating the Timestamp of Your Latest iPhone iCloud Sync: A Comprehensive Tutorial for Users and Administrators</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/new-in-2024-unlock-efficient-video-editing-6-essential-adobe-premiere-pro-tips/"><u>New In 2024, Unlock Efficient Video Editing 6 Essential Adobe Premiere Pro Tips</u></a></li>
<li><a href="https://win-webster.techidaily.com/step-by-step-tutorial-on-retrieving-accidentally-deleted-rmvb-videos/"><u>Step-by-Step Tutorial on Retrieving Accidentally Deleted RMVB Videos</u></a></li>
<li><a href="https://win-webster.techidaily.com/top-pfechten-pc-klonierungssoftware-fur-windows-11-10-and-8-ihre-endgultige-losung/"><u>Top-PFechten PC-Klonierungssoftware Für Windows 11, 10 & 8: Ihre Endgültige Lösung</u></a></li>
<li><a href="https://games-able.techidaily.com/troubleshooting-steam-big-picture-and-solving-problems/"><u>Troubleshooting Steam Big Picture and Solving Problems</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2123512/26400" target="_top" id="2123512">
  <img src="//a.impactradius-go.com/display-ad/26400-2123512" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2123512/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

