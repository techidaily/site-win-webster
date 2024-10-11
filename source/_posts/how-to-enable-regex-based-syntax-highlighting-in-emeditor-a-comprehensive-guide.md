---
title: "How to Enable Regex-Based Syntax Highlighting in EmEditor: A Comprehensive Guide"
date: 2024-10-07T06:09:38.002Z
updated: 2024-10-11T01:54:00.648Z
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
<li><a href="https://visual-screen-recording.techidaily.com/new-exploring-whether-itop-fits-your-tech-needs/"><u>[New] Exploring Whether ITop Fits Your Tech Needs</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-in-2024-premier-portals-to-retro-playstation-gaming-on-your-desktop/"><u>[New] In 2024, Premier Portals to Retro PlayStation Gaming on Your Desktop</u></a></li>
<li><a href="https://win-webster.techidaily.com/big-news-exciting-windows-on-arm-applications-arrive-why-it-matters-technewsz/"><u>Big News: Exciting Windows on ARM Applications Arrive – Why It Matters | TechNewsZ</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/comprehensive-list-of-top-9-free-video-channel-branding-aids/"><u>Comprehensive List of Top 9 Free Video Channel Branding Aids</u></a></li>
<li><a href="https://blog-min.techidaily.com/conversao-livre-em-linha-para-formatos-video-rmvb-flv-com-o-aplicativo-movavi/"><u>Conversão Livre Em Linha Para Formatos Video (RMVB, FLV) Com O Aplicativo Movavi</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/efficient-methods-for-converting-m2p-videos-into-mp4-a-comprehensive-guide/"><u>Efficient Methods for Converting M2P Videos Into MP4: A Comprehensive Guide</u></a></li>
<li><a href="https://win-webster.techidaily.com/microsoft-revises-consumer-strategy-approach-once-more-insights-from-zdnet/"><u>Microsoft Revises Consumer Strategy Approach Once More - Insights From ZDNet</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/prime-fareless-streaming-and-recording-software/"><u>Prime Fareless Streaming & Recording Software</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/n-tactics-to-amplify-your-youtube-popularity/"><u>Proven Tactics to Amplify Your YouTube Popularity</u></a></li>
<li><a href="https://article-files.techidaily.com/unleash-creativity-in-memes-genrator-assistance-for-2024/"><u>Unleash Creativity in Memes Gen'rator Assistance for 2024</u></a></li>
<li><a href="https://win-webster.techidaily.com/unveiling-the-dynamic-between-openai-and-microsoft-collaborative-giants-or-silicon-valley-rivals/"><u>Unveiling the Dynamic Between OpenAI and Microsoft - Collaborative Giants or Silicon Valley Rivals?</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/visionary-tech-review-the-video-hub/"><u>Visionary Tech Review The Video Hub</u></a></li>
<li><a href="https://win-webster.techidaily.com/windows-elite-unveiling-the-power-of-microsoft-surface-pro-9-as-a-true-contender-to-the-macbook-insider-review-by-zdnet/"><u>Windows Elite: Unveiling the Power of Microsoft Surface Pro 9 as a True Contender to the MacBook | Insider Review by ZDNet</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075475/7443" target="_top" id="2075475">
  <img src="//a.impactradius-go.com/display-ad/7443-2075475" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075475/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

