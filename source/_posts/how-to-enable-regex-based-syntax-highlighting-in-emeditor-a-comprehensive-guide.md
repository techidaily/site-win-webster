---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-10-12T16:09:25.268Z
updated: 2024-10-17T16:11:47.494Z
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
<li><a href="https://twitter-clips.techidaily.com/new-screen-scores-viral-video-highlights-on-twitter-for-2024/"><u>[New] Screen Scores Viral Video Highlights on Twitter for 2024</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/new-top-10-must-haves-action-cameras-unleashed/"><u>[New] Top 10 Must-Haves Action Cameras Unleashed</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/updated-2024-approved-enhancing-gaming-experience-minecraft-recordings-made-easy/"><u>[Updated] 2024 Approved Enhancing Gaming Experience Minecraft Recordings Made Easy</u></a></li>
<li><a href="https://win-webster.techidaily.com/1-regang-regokan-kartu-memo-jadi-pembantu-gratis-untuk-menyimpan-data-anda/"><u>1. Regang-Regokan Kartu Memo: Jadi Pembantu Gratis Untuk Menyimpan Data Anda</u></a></li>
<li><a href="https://win-webster.techidaily.com/1728484824784-aomei-onebackup/"><u>一體化雲端儲存及網站全面備份管理 - AOMEI OneBackup</u></a></li>
<li><a href="https://win-webster.techidaily.com/comprendre-la-suppression-de-windows-easy-transfer-dans-les-dernieres-versions-de-windows-11/"><u>Comprendre La Suppression De Windows Easy Transfer Dans Les Dernières Versions De Windows 11</u></a></li>
<li><a href="https://win-webster.techidaily.com/download-the-latest-emeditor-pro-700-pre-release-leading-text-editor-software/"><u>Download the Latest EmEditor Pro 7.00 Pre-Release - Leading Text Editor Software</u></a></li>
<li><a href="https://win-webster.techidaily.com/effective-solutions-when-your-new-iphone-fails-to-retrieve-a-backup-during-initial-configuration/"><u>Effective Solutions When Your New iPhone Fails to Retrieve a Backup During Initial Configuration</u></a></li>
<li><a href="https://win-webster.techidaily.com/guida-dettagliata-a-inviare-correttamente-lemail-da-outlook-su-un-computer-mac-consigli-e-suggerimenti-essenziali/"><u>Guida Dettagliata a Inviare Correttamente L'Email Da Outlook Su Un Computer Mac: Consigli E Suggerimenti Essenziali</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-use-ispoofer-on-vivo-s18e-drfone-by-drfone-virtual-android/"><u>How to use iSpoofer on Vivo S18e? | Dr.fone</u></a></li>
<li><a href="https://windows11.techidaily.com/quick-glances-to-your-favorites-windows-shortcuts-uwp-apps/"><u>Quick Glances to Your Favorites: Windows Shortcuts (UWP Apps)</u></a></li>
<li><a href="https://driver-download.techidaily.com/quick-guide-fresh-asus-dvd-driver-download-and-installation-steps/"><u>Quick Guide: Fresh ASUS DVD Driver Download and Installation Steps</u></a></li>
<li><a href="https://win-webster.techidaily.com/resolved-how-to-remove-partitions-in-windows-10/"><u>Resolved: How to Remove Partitions in Windows 10</u></a></li>
<li><a href="https://win-blog.techidaily.com/resolving-the-issue-understanding-and-fixing-apex-legends-error-23/"><u>Resolving the Issue: Understanding and Fixing Apex Legends Error 23</u></a></li>
<li><a href="https://win-webster.techidaily.com/sauvegardez-avec-assurance-guide-complet-a-trois-etapes-pour-disque-dur-externe/"><u>Sauvegardez Avec Assurance : Guide Complet À Trois Étapes Pour Disque Dur Externe</u></a></li>
<li><a href="https://win-webster.techidaily.com/tiga-langkah-gratis-untuk-mengenali-dan-menemukan-file-yang-hapus-abad-ke-3/"><u>Tiga Langkah Gratis Untuk Mengenali Dan Menemukan File Yang Hapus Abad Ke-3</u></a></li>
<li><a href="https://activate-lock.techidaily.com/unlock-your-device-icloud-dns-bypass-explained-and-tested-plus-easy-alternatives-on-iphone-11-by-drfone-ios/"><u>Unlock Your Device iCloud DNS Bypass Explained and Tested, Plus Easy Alternatives On iPhone 11</u></a></li>
<li><a href="https://win-studio.techidaily.com/upgrading-to-windows-11-without-cost-current-status-explained-by-zdnet/"><u>Upgrading to Windows 11 Without Cost: Current Status Explained by ZDNet</u></a></li>
<li><a href="https://solve-news.techidaily.com/windows-10-dvd-dvd/"><u>Windows 10 DVD再生可能化ガイド: DVDプレイヤー用フォーマットで確実に作成する方法</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135365/19272" target="_top" id="2135365">
  <img src="//a.impactradius-go.com/display-ad/19272-2135365" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135365/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

