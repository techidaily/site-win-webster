---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-10-20T01:29:32.223Z
updated: 2024-10-23T04:57:12.956Z
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
<li><a href="https://youtube-stream.techidaily.com/2024-approved-from-raw-footage-to-polished-content-youtube-studio-edition/"><u>2024 Approved From Raw Footage to Polished Content YouTube Studio Edition</u></a></li>
<li><a href="https://win-webster.techidaily.com/building-an-emachines-recovery-disk-in-various-windows-os-quick-guide-for-win7-to-win11-using-two-proven-techniques/"><u>Building an eMachines Recovery Disk in Various Windows OS: Quick Guide for Win7 to Win11 Using Two Proven Techniques</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/catch-or-beat-sleeping-snorlax-on-pokemon-go-for-apple-iphone-x-drfone-by-drfone-virtual-ios/"><u>Catch or Beat Sleeping Snorlax on Pokemon Go For Apple iPhone X | Dr.fone</u></a></li>
<li><a href="https://techtrends.techidaily.com/essential-fixes-for-a-broken-macbook-pro-keyboard-what-you-need-to-know/"><u>Essential Fixes for a Broken MacBook Pro Keyboard – What You Need to Know</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-8-best-apps-for-screen-mirroring-tecno-camon-20-pro-5g-pc-drfone-by-drfone-android/"><u>In 2024, 8 Best Apps for Screen Mirroring Tecno Camon 20 Pro 5G PC | Dr.fone</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-how-to-lock-apps-on-oneplus-ace-2-pro-to-protect-your-individual-information-by-drfone-android/"><u>In 2024, How to Lock Apps on OnePlus Ace 2 Pro to Protect Your Individual Information</u></a></li>
<li><a href="https://win11.techidaily.com/lowering-pc-resource-demand-fixing-wmi-usage-issues/"><u>Lowering PC Resource Demand: Fixing WMI Usage Issues</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/seamless-xp-pen-driver-update-techniques-explained/"><u>Seamless XP-Pen Driver Update Techniques Explained</u></a></li>
<li><a href="https://win-webster.techidaily.com/strategies-pour-recuperer-vos-fichiers-perdus-suite-a-linstallation-de-windows-11-guide-pratique-avec-5-techniques/"><u>Stratégies Pour Récupérer Vos Fichiers Perdus Suite À L'Installation De Windows 11 - Guide Pratique Avec 5 Techniques</u></a></li>
<li><a href="https://win-webster.techidaily.com/top-7-solutions-for-resolving-the-disk-read-error-on-windows-versions-11-7-8-and-xp/"><u>Top 7 Solutions for Resolving the 'Disk Read Error' On Windows Versions 11, 7, 8 & XP</u></a></li>
<li><a href="https://win-webster.techidaily.com/top-rated-wd-hard-drive-copying-tools-ultimate-guide-on-how-to-perform-a-perfect-wd-ssd-clone/"><u>Top-Rated WD Hard Drive Copying Tools: Ultimate Guide on How To Perform a Perfect WD SSD Clone</u></a></li>
<li><a href="https://win-webster.techidaily.com/44oh44k544kv44oi44od44ox44gn44k344on44o844oi44kr44od44oi44gq44gp44gq44gj44gm44gx44gplus44ge44gplus44gx44gf44cc6kej5rg65pa55rov77yw44gk44gu57s55lul/"><u>デスクトップでショートカットなくなってしまいました。解決方法６つご紹介</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/1001446/11832" target="_top" id="1001446">
  <img src="//a.impactradius-go.com/display-ad/11832-1001446" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1001446/11832" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

