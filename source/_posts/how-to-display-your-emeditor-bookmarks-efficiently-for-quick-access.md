---
title: How to Display Your EmEditor Bookmarks Efficiently for Quick Access
date: 2024-10-05T17:45:08.342Z
updated: 2024-10-11T03:11:25.022Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/5f63ba1e3593ebd7d73d1c72fb68eace0cd63a5c8a537d585a504e6de4ee75de.jpg
---

## How to Display Your EmEditor Bookmarks Efficiently for Quick Access

Viewing 1 post (of 1 total)

* Author  
Posts
* October 5, 2008 at 2:16 am [#6315](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
Show list of bookmarks in document (VBScript)  
**Provided “as is”. No guaranty.**  
 **Test first on non important documents! I am no programmer.**  
 **Please comment below how it works.**  
 I have missed this feature under “Edit > Bookmarks”  
 and ‘cus i want to play with macro language  
 i decide to make this macro.  
 (I think such an option should be there in that menu?)  
 See EmEditor Help for how to use macros. Here’s an short help:  
 1.) Save the code between 8< and >8 -lines as text file “somename.vbee” in EmEditor folder  
 2.) use Menu “Macros > Select…” and choose this somename.vbee as current default macro  
 3.) open an test file (try first on an test document!)  
 and create some bookmarks with Strg+F2  
 4.) press F4  
 5.) you are prompted with an list of all bookmarks and the line contend at bookmarked line  
 Your done.  
 ———–8<---------------8<-----------  
    
	#title = Bookmark List  
	#tooltip = Show list of bookmarks in document  
	'//  
	'//  
	'------------------------------------------------------Prepare work  
	Set WshShell = CreateObject("WScript.Shell")  
	maxCount = 50 								'how many output lines to Display	due window hight  
	StartLine = document.selection.GetActivePointY (eePosView)		'get and store start parameters  
	StartColumn = document.selection.GetActivePointx (eePosView)  
	document.selection.SetActivePoint eePosView, 1, 1				'go to top of file  
	'------------------------------------------------------Work  
	    
	Do  
		FindNextBookmark = document.selection.NextBookmark  
		If FindNextBookmark = TRUE THEN  
			Count = Count + 1  
			NextBookmark = document.selection.GetActivePointY (eePosView) 'get line number and contend  
			str = document.GetLine (NextBookmark)  
			If Count < maxCount +1 THEN									'collect all info for output  
				BookmarkCollect =  BookmarkCollect & vbCRLF & Count& "  Line " & NextBookmark & ": " & vbTab & str  
			End IF  
		End IF  
	LOOP UNTIL (FindNextBookmark  = FALSE)  
	document.selection.SetActivePoint eePosView, StartColumn, StartLine		'go back to start line  
	'------------------------------------------------------Prepare output  
	If Count > maxCount THEN  
		result = maxCount  
		resText = result & " of " & Count & " bokmarks listed only, due settings in script because of hight of this dialog."  
	ELSE  
		result = Count  
		resText = "All " & Count & " bokmarks listed."  
	End IF  
	InfoText = "Use 'Strg+G' to jump to line."  
	'------------------------------------------------------Output Messagebox. Use Strg+G to go to line  
	If Count > 0 THEN  
	    n = WshShell.Popup(BookmarkCollect & vbCRLF & vbCRLF & resText & vbCRLF & InfoText, , "List of bookmarks", 0)  
	ELSE  
	    n = WshShell.Popup("No bookmarks found in this document.", , "List of bookmarks", 0)  
	End IF  
	    
	    
	 ———–>8—————>8———–  
 Settings:  
 see “maxCount = 50 ”  
 Default it will show the first 50 bookmarks only.  
 Set it to your need.  
 Test if the hight of the dialog box fit to your screen.  
 Enjoy  
 Stefan  
 Comments and improvement suggestion welcome.
* Author  
Posts

Viewing 1 post (of 1 total)

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
<li><a href="https://desktop-recording.techidaily.com/new-2024-approved-decoding-ios-digital-screen-snatcher-secrets/"><u>[New] 2024 Approved Decoding IO's Digital Screen Snatcher Secrets</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-easy-listening-top-hits-from-facebook/"><u>[Updated] Easy Listening Top Hits From Facebook</u></a></li>
<li><a href="https://win-webster.techidaily.com/a-step-by-step-guide-viewing-your-flipbooks-anywhere-with-mobile-compatibility-flipbuildercom/"><u>A Step-by-Step Guide: Viewing Your FlipBooks Anywhere with Mobile Compatibility - flipbuilder.com</u></a></li>
<li><a href="https://win-webster.techidaily.com/adjusting-flipbuilders-bottom-menu-hue-a-comprehensive-tutorial/"><u>Adjusting FlipBuilder's Bottom Menu Hue: A Comprehensive Tutorial</u></a></li>
<li><a href="https://win-webster.techidaily.com/are-mac-users-supported-by-flipbuilder-find-out-now/"><u>Are Mac Users Supported by FlipBuilder - Find Out Now!</u></a></li>
<li><a href="https://win-webster.techidaily.com/beginners-guide-to-opening-with-a-slider-view-in-flipbuilder-craft-impressive-thumbnails-from-the-start/"><u>Beginner's Guide to Opening with a Slider View in FlipBuilder – Craft Impressive Thumbnails From the Start</u></a></li>
<li><a href="https://win-webster.techidaily.com/build-a-stunning-web-published-flipbook-with-html-a-step-by-step-guide-using-flipbuilder/"><u>Build a Stunning Web-Published Flipbook with HTML: A Step-by-Step Guide Using FlipBuilder</u></a></li>
<li><a href="https://tech-haven.techidaily.com/convert-videos-flawlessly-top-free-mp4-tools-for-your-amazon-kindle-fire-device/"><u>Convert Videos Flawlessly - Top Free MP4 Tools for Your Amazon Kindle Fire Device</u></a></li>
<li><a href="https://win-webster.techidaily.com/convert-your-pdfs-into-a-professional-slideshow-with-our-free-pdf-to-flipbook-tool/"><u>Convert Your PDFs Into a Professional Slideshow with Our Free PDF-to-Flipbook Tool</u></a></li>
<li><a href="https://video-capture.techidaily.com/discover-the-hidden-path-resolved-errors-with-wonderfoxs-expertise/"><u>Discover the Hidden Path: Resolved Errors with WonderFox's Expertise</u></a></li>
<li><a href="https://win-howtos.techidaily.com/diuril-ibuprofen-and-lipitor-in-that-order/"><u>Diuril, Ibuprofen, and Lipitor in that Order</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/expert-chromebook-zoom-techniques-unveiled/"><u>Expert Chromebook Zoom Techniques Unveiled</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/in-2024-premium-free-graphic-havens-a-comprehensive-guide-to-top-art-portals/"><u>In 2024, Premium-Free Graphic Havens A Comprehensive Guide to Top Art Portals</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-why-your-whatsapp-location-is-not-updating-and-how-to-fix-on-motorola-moto-e13-drfone-by-drfone-virtual-android/"><u>In 2024, Why Your WhatsApp Location is Not Updating and How to Fix On Motorola Moto E13 | Dr.fone</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/leading-server-racks-and-closure-units-of-the-year-2024-edition/"><u>Leading Server Racks and Closure Units of the Year: 2024 Edition</u></a></li>
<li><a href="https://win-webster.techidaily.com/step-by-step-guide-to-upload-and-modify-your-design-on-flipprogram-flipbuildercom/"><u>Step-by-Step Guide to Upload and Modify Your Design on FlipProgram (flipbuilder.com)</u></a></li>
<li><a href="https://win-webster.techidaily.com/transform-pdf-and-various-image-formats-into-stunning-android-books-with-flipbuilder/"><u>Transform PDF & Various Image Formats Into Stunning Android Books with FlipBuilder</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2098705/14409" target="_top" id="2098705">
  <img src="//a.impactradius-go.com/display-ad/14409-2098705" border="0" alt="https://techidaily.com" width="250" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2098705/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

