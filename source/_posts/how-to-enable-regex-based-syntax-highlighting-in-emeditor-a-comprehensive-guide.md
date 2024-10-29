---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-10-26T02:04:05.172Z
updated: 2024-10-28T17:09:44.566Z
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
<li><a href="https://fox-helps.techidaily.com/new-revealed-top-5-ingenious-whatsapp-shortcuts-for-2024/"><u>[New] Revealed Top 5 Ingenious WhatsApp Shortcuts for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-in-2024-bypass-software-for-youtube-downloads/"><u>[Updated] In 2024, Bypass Software for YouTube Downloads</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ed-integrating-video-content-youtube-and-google-slides/"><u>[Updated] Integrating Video Content YouTube & Google Slides</u></a></li>
<li><a href="https://win-webster.techidaily.com/1-pasos-faciles-para-mover-archivos-de-windows-a-macos-sin-usar-migration-assistant/"><u>1. 'Pasos Fáciles Para Mover Archivos De Windows a macOS Sin Usar Migration Assistant'</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-how-to-convert-avi-to-gif-on-windows-and-mac-with-filmora/"><u>2024 Approved How to Convert AVI to GIF on Windows & Mac with Filmora</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-premier-tools-for-image-transformation-framecraft-pro/"><u>2024 Approved Premier Tools for Image Transformation FrameCraft Pro</u></a></li>
<li><a href="https://win-webster.techidaily.com/1728501401757-windows-10-usb/"><u>適用於Windows 10的外置 USB 自動儲存便攜解決方案</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/a-step-by-step-guide-on-using-adb-and-fastboot-to-remove-frp-lock-from-your-vivo-s18e-by-drfone-android/"><u>A Step-by-Step Guide on Using ADB and Fastboot to Remove FRP Lock from your Vivo S18e</u></a></li>
<li><a href="https://win-webster.techidaily.com/guide-pratique-reinitialiser-completement-windows/"><u>Guide Pratique : Réinitialiser Complètement Windows</u></a></li>
<li><a href="https://win-webster.techidaily.com/kontinuierliche-datenwiederherstellung-schritt-fur-schritt-anleitung-fur-windows-11-10-8-und-7/"><u>Kontinuierliche Datenwiederherstellung: Schritt-Für-Schritt-Anleitung Für Windows 11, 10, 8 Und 7</u></a></li>
<li><a href="https://win-webster.techidaily.com/les-3-meilleurs-metodos-simples-pour-fabriquer-un-hdd-extern-seuil-amovible/"><u>Les 3 Meilleurs Métodos Simples Pour Fabriquer Un HDD Extern Seuil Amovible</u></a></li>
<li><a href="https://win-help.techidaily.com/movavi-media-player-a-secure-software-solution-for-multimedia-playback/"><u>Movavi Media Player: A Secure Software Solution for Multimedia Playback</u></a></li>
<li><a href="https://win-webster.techidaily.com/overcoming-file-migration-challenges-on-a-mac-to-usb-step-by-step-correction-guide/"><u>Overcoming File Migration Challenges on a Mac to USB – Step-by-Step Correction Guide</u></a></li>
<li><a href="https://win-webster.techidaily.com/schutz-von-windows-11-laufwerks-c-zwei-optimierte-ansatze-erklart/"><u>Schutz Von Windows 11 Laufwerks C: Zwei Optimierte Ansätze Erklärt</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/snapdragon-laptop-reviews-in-action-exclusive-live-coverage-and-impressions/"><u>Snapdragon Laptop Reviews in Action: Exclusive Live Coverage and Impressions</u></a></li>
<li><a href="https://blue-screen-error.techidaily.com/solving-the-nvpcfsys-bsod-issue-step-by-step-guide/"><u>Solving the nvpcf.sys BSoD Issue: Step-by-Step Guide</u></a></li>
<li><a href="https://win-webster.techidaily.com/top-empfohlene-grossrechner-datensicherungsprogramme-fur-geschaftskunden-und-it-dienstleister/"><u>Top-Empfohlene Großrechner-Datensicherungsprogramme Für Geschäftskunden Und IT-Dienstleister</u></a></li>
<li><a href="https://win-howtos.techidaily.com/troubleshooting-missing-modules-in-your-system-expert-solutions/"><u>Troubleshooting Missing Modules in Your System – Expert Solutions</u></a></li>
<li><a href="https://win-webster.techidaily.com/win10-drawer-gone-crisis-solution-unlocked-free-detailed-recovery-manual/"><u>Win10 Drawer Gone? Crisis Solution Unlocked! Free Detailed Recovery Manual</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1868575/19272" target="_top" id="1868575">
  <img src="//a.impactradius-go.com/display-ad/19272-1868575" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1868575/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

