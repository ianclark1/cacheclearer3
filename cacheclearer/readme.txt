

INSTALL

Extract the zip into a temporary folder. Next find your ColdFusion Administrator. This is typically 
located under your web root at: /CFIDE/admistrator. Create a new folder called cacheclearer. Copy 
the files into this folder. (You do not need to copy this file or the readme.txt file of course.) 

In the root folder of the ColdFusion Administrator, you may or may not see a file called 
custommenu.xml.Open the file and add this text:

<submenu label="My Tools">
	<menuitem href="cacheclearer/" target="content">CacheClearer</menuitem>
</submenu>

You can name the submenu anything you want. If you already have a custom menu, you can simply add the menu item. 
This file simply tells the ColdFusion Administrator to add a custom link. Save the file. 


Open the ColdFusion Administrator in your browser. In the left hand menu, you should see a section 
named My Tools. Click the arrow to expand it, and you should see a link called CacheCleaner. Click
the link and the tool will load. 

==========================================================================
HISTORY

Version 1.2 - May 25, 2010
Remembers your last 5 paths.

Version 1.1 - April 2, 2009
Mods by Eric P. Supports checking to see if trusted cache is even enabled. If not, the form is disabled.

Version 1.1 - April 2, 2009
Mods by Eric P. Supports list of files separated by a comma, and optionally recursing directories. 
Mod by Yaron Kohn to use a cookie to tell CF Admin this was your last page.