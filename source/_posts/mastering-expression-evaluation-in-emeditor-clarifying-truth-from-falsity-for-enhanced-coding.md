---
title: "Mastering Expression Evaluation in EmEditor: Clarifying Truth From Falsity for Enhanced Coding"
date: 2024-10-05T21:15:25.809Z
updated: 2024-10-10T18:24:52.918Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/cf29c28ece4619a4babae69368aabca262cca3e6476270a9e9bd6f5a744eb780.jpg
---

## Mastering Expression Evaluation in EmEditor: Clarifying Truth From Falsity for Enhanced Coding

Viewing 7 posts - 1 through 7 (of 7 total)

* Author  
Posts
* October 14, 2011 at 6:51 am [#9732](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
How can i utilize this feature please?  
**(?n:true\_expression:false\_expression)**  
 Found at:  
[http://www.emeditor.com/modules/feature1/rewrite/tc\_35.html](https://tools.techidaily.com/emeditor/products/)  
 EmEditor Professional 9 New Features  
 The replace format “(?n:true\_expression:false\_expression)”  
 was added to regular expression replace formats.  
October 17, 2011 at 8:10 pm [#9741](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/99e0a4de99febcf136998ab176c8b5aa?s=80&d=identicon&r=g)JohnQSmith](https://www.emeditor.com/forums/users/johnqsmith/ "View JohnQSmith's profile")  
Participant  
I played with it a while and finally figured it out. Here’s an example.  
 Input document  
TheGreenAile TheGreenBile TheGreenCile TheGreenDile  
	TheGreenEile TheGreenFile TheGreenGile TheGreenHile  
	TheGreenIile TheGreenJile TheGreenKile TheGreenLile  
	TheGreenNile TheGreenOile TheGreenPile TheGreenQile  
	TheGreenRile TheGreenSile TheGreenUile TheGreenVile  
	TheGreenWile TheGreenXile TheGreenYile TheGreenZile  
	 Search string  
**(?:([BFNPR])|([^BFNPR]))(ile)**  
	 Replace string  
**(?1:M:T)3**  
 Replace all and output is  
TheGreenTile TheGreenMile TheGreenTile TheGreenTile  
	TheGreenTile TheGreenMile TheGreenTile TheGreenTile  
	TheGreenTile TheGreenTile TheGreenTile TheGreenTile  
	TheGreenMile TheGreenTile TheGreenMile TheGreenTile  
	TheGreenMile TheGreenTile TheGreenTile TheGreenTile  
	TheGreenTile TheGreenTile TheGreenTile TheGreenTile  
 I color coded it to help you see what’s happening.  
 Oh yeah, the [Boost](http://www.boost.org/doc/libs/1%5F47%5F0/libs/regex/doc/html/boost%5Fregex/format/boost%5Fformat%5Fsyntax.html) regex docs helped me figure it out.  
October 18, 2011 at 5:46 am [#9742](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
 Thanks John!  
 I see it, but i don’t understand it.  
 Will have an closer look and read the Boost help…  
October 18, 2011 at 7:18 am [#9743](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
> Conditionals  
> The character ‘?’ begins a conditional expression, the general form is:  
> ?Ntrue-expression:false-expression  
> where N is decimal digit.  
> If sub-expression N was matched, then true-expression is evaluated and sent to output,  
> otherwise false-expression is evaluated and sent to output.  
> You will normally need to surround a conditional-expression with parenthesis in order to prevent ambiguities.  
> For example, the format string “(?1foo:bar)” will replace each match found with “foo” if the sub-expression $1 was matched,  
> and with “bar” otherwise.  
> For sub-expressions with an index greater than 9, or for access to named sub-expressions use:  
> ?{INDEX}true-expression:false-expression  
> or  
> ?{NAME}true-expression:false-expression  
>  
> conditional expression ?Ntrue-expression:false-expression  
>  
> In addition, conditional expressions of the following form are recognized:  
> ?Ntrue-expression:false-expression  
> where N is a decimal digit representing a sub-match.  
> If the corresponding sub-match participated in the full match, then the substitution is true-expression.  
> Otherwise, it is false-expression. In this mode, you can use parens () for grouping.  
> If you want a literal paren, you must escape it as (.  
 Seams clear, but i have still problems using this.  
 Some tests:  
    
	conditional expression  
	'?Ntrue-expression:false-expression' test 1  
	    
	I have:  
	Test Price 1000  
	Test Price 100  
	Test Price 800  
	---  
	Find: (.+) (.+) (d{3})(d)  
	Replace: (?4: too expensive: affordable)  
	[X] Use RegEx  
	---  
	Result:  
	Test Price 1000 too expensive  
	Test Price 100  
	Test Price 800  
	---  
	Expected:  
	Test Price 1000 too expensive  
	Test Price 100 affordable  
	Test Price 800 affordable  
	---  
	Explanation:  
	If sub-expression No. 4 match THEN  
	use 'true-expression'  
	else 'false-expression'  
	    
	conditional expression  
	'?Ntrue-expression:false-expression' test 2  
	    
	I have:  
	Color 1 green  
	Color 2 blue  
	Color 3 red  
	The available colors are either green, blue or red.  
	---  
	Find: (Color d) (.+)  
	Replace: (?1:1 2-ich:1 -2-)  
	[X] Use RegEx  
	---  
	Result:  
	Color 1 green-ich  
	Color 2 blue-ich  
	Color 3 red-ich  
	The available colors are either green, blue or red.  
	---  
	Expected:  
	Color 1 green-ich  
	Color 2 blue-ich  
	Color 3 red-ich  
	The available colors are either -green-, -blue- or -red-.  
	---  
	Explanation:  
	Only if sub-expression No. 1 will match THEN  
	use 'true-expression'  
	else 'false-expression'  
	 OK, i will test some more.  
October 18, 2011 at 2:39 pm [#9744](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/99e0a4de99febcf136998ab176c8b5aa?s=80&d=identicon&r=g)JohnQSmith](https://www.emeditor.com/forums/users/johnqsmith/ "View JohnQSmith's profile")  
Participant  
I see the problem with both of your tests. It’s the same thing that took me so long to figure out how it works.  
 Here’s the key…  
 The whole RegEx must match in order for it to work. In other words, you have to set up the RegEx with an alternation so that it has **both a success and a failure point**.  
 In your first test, only the first line matched your RegEx (I’m using underscores as filler to demonstrate).  
    
	Test Price 100______0  
	(.+) (.+)  (d{3}) (d)   <-- this matches  
	    
	Test Price 100________  
	(.+) (.+)  (d{3}) (d)   <-- this doesn't match, there is no final (d)  
	    
	Test Price 800________  
	(.+) (.+)  (d{3}) (d)   <-- also doesn't match  
	 Here’s how I changed your RegEx to work.  
    
	        Note the success ----.  and failure points  
	                             |  |  
	                             v  v  
	Find: ^(.+) (.+) (d{3})(?:(d)|$)  
	Replace:  (?4:too expensive:affordable)  
 Your second example is the same thing.  
    
	Color_ 1__ green  
	(Color d) (.+)   <-- match  
	    
	Color_ 2__ blue  
	(Color d) (.+)   <-- match  
	    
	Color_ 3__ red  
	(Color d) (.+)   <-- match  
	    
	The available colors are either green, blue or red.  
	(Color d) (.+)   <-- no match anywhere on line  
	 Hope this helps.  
October 18, 2011 at 6:12 pm [#9745](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
Thank you.  
 My understanding right now:  
 You have to set up the FIND RegEx with an alternation so that it has both a success and a failure point.  
 As the REPLACE have too possibilities too: (?n:true\_expression:false\_expression)  
 Test:  
    
	I have:  
	Test Price 1000  
	Test Price 100  
	Test Price 800  
	    
	Find: (.+) (.+) (d{3})(d)*  
	Repl: (?4: too expensive: affordable)  
	[X] Use RegEx  
	    
	Result:  
	Test Price 1000 too expensive  
	Test Price 100 affordable  
	Test Price 800 affordable  
 Thanks again. I still have to do some test, but i think you showed me the way.  
 –  
 BTW, good idea :lol: of you:  
 Replace: (?4:too expensive:affordable)  
 –  
October 18, 2011 at 6:39 pm [#9746](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/99e0a4de99febcf136998ab176c8b5aa?s=80&d=identicon&r=g)JohnQSmith](https://www.emeditor.com/forums/users/johnqsmith/ "View JohnQSmith's profile")  
Participant  
> My understanding right now:  
> You have to set up the FIND RegEx with an alternation so that it has both a success and a failure point.  
> As the REPLACE have too possibilities too: (?n:true\_expression:false\_expression)  
 Absolutely correct. I like your FIND RegEx better. It will be much easier to use than mine. Just adding the zero or more switch makes it much simpler than a non-matching alternation grouping.  
 What helped me the most in figuring out how it works was how EmEditor highlights all matches when you do a search. When I tried your first search, only the first “Test Price” line was highlighted, but when I removed the final “(d)”, all the lines were marked. This showed me that the problem was with the RegEx.  
 The first and foremost thing to remember is that the WHOLE RegEx expression must match before you can do any further matching and testing with a SUBexpression.  
> BTW, good idea :lol: of you:  
> Replace: (?4:too expensive:affordable)  
 Thanks! :-D
* Author  
Posts

Viewing 7 posts - 1 through 7 (of 7 total)

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
<li><a href="https://instagram-videos.techidaily.com/new-mastering-the-art-of-cinematic-content-on-instagram/"><u>[New] Mastering the Art of Cinematic Content on Instagram</u></a></li>
<li><a href="https://fox-direct.techidaily.com/updated-2024-approved-the-editors-pathway-for-diminishing-sound-levels/"><u>[Updated] 2024 Approved The Editor's Pathway for Diminishing Sound Levels</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-a-compre-market-leaders-guide-to-the-most-effective-fb-video-ad-approaches-for-2024/"><u>[Updated] A Compre Market Leader's Guide to the Most Effective FB Video Ad Approaches for 2024</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-deep-dive-into-the-best-ways-to-speed-up-facebook-videos/"><u>[Updated] Deep Dive Into The Best Ways to Speed Up Facebook Videos</u></a></li>
<li><a href="https://extra-support.techidaily.com/updated-perfecting-small-details-on-google-meet-screen/"><u>[Updated] Perfecting Small Details on Google Meet Screen</u></a></li>
<li><a href="https://win-webster.techidaily.com/a-step-by-step-guide-viewing-your-flipbooks-anywhere-with-mobile-compatibility-flipbuildercom/"><u>A Step-by-Step Guide: Viewing Your FlipBooks Anywhere with Mobile Compatibility - flipbuilder.com</u></a></li>
<li><a href="https://win-webster.techidaily.com/adjusting-flipbuilders-bottom-menu-hue-a-comprehensive-tutorial/"><u>Adjusting FlipBuilder's Bottom Menu Hue: A Comprehensive Tutorial</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/best-of-the-best-10-recorders-for-your-device-for-2024/"><u>Best of the Best #10 Recorders for Your Device for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/getting-acquainted-the-google-meet-pathway-for-2024/"><u>Getting Acquainted The Google Meet Pathway for 2024</u></a></li>
<li><a href="https://fix-guide.techidaily.com/how-to-fix-part-of-the-touch-screen-not-working-on-samsung-galaxy-s23-fe-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How To Fix Part of the Touch Screen Not Working on Samsung Galaxy S23 FE | Dr.fone</u></a></li>
<li><a href="https://win-webster.techidaily.com/step-by-step-guide-to-upload-and-modify-your-design-on-flipprogram-flipbuildercom/"><u>Step-by-Step Guide to Upload and Modify Your Design on FlipProgram (flipbuilder.com)</u></a></li>
<li><a href="https://win-webster.techidaily.com/transform-pdf-and-various-image-formats-into-stunning-android-books-with-flipbuilder/"><u>Transform PDF & Various Image Formats Into Stunning Android Books with FlipBuilder</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1880927/19272" target="_top" id="1880927">
  <img src="//a.impactradius-go.com/display-ad/19272-1880927" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1880927/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

