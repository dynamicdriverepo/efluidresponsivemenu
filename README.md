# eFluid Responsive Top Menu #

*Description:* Inspired by the drop down menu seen at the top of pages throughout [Dynamic Drive](http://dynamicdrive.com/),  eFluid menu is a responsive top menu that adapts to different devices and screen sizes elegantly, using CSS  media queries only to trigger the different break points. Go from a fully equip top menu bar on large screen devices, a two line menu on smaller screens, to a mobile optimized "hamburger" menu on mobile devices. The menu supports a single level of drop down menus, including arbitrary HTML, multicolumn sub menus.

## Directions ##

Add the following code to the HEAD of your page:

	<link rel="stylesheet" type="text/css" href="assets/efluidmenu.css" />
	
	<!--[if lte IE 8]>
	<style type="text/css">
	
	.efluidmenu > ul{
				margin-left: 55px;
	}
	
	.efluidmenu > ul li#search{
				display: none;
	}
	
		.efluidmenu #sitelogo {
		    left: 0;  /* position logo to the very left of menu in IE8 and below */
		}
		
		.efluidmenu #sitelogo a {
		    left: auto;
		}
	
	</style>   
	<![endif]-->
	
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
	
	<script src="assets/efluidmenu.js">
	
	/***********************************************
	* eFluid Menu script (c) Dynamic Drive (www.dynamicdrive.com)
	* Please keep this notice intact
	* Visit http://www.dynamicdrive.com/ for this script and 100s more.
	***********************************************/
	
	</script>

## Menu Markup ##

Add the following sample menu markup to your page:

	<div id="fluidmenu1" class="efluidmenu">
	
	<a class="efluid-animateddrawer" href="#">
	<span></span>
	</a>
	
	<ul>
	<li id="sitelogo"><a href="http://www.dynamicdrive.com/"><img border="0" src="assets/ddlogov2.png"></a></li>
	<li><a href="http://www.google.com">Item 1</a></li>
	<li><a href="http://www.google.com">Folder 0</a>
	  <ul>
	  <li><a href="http://www.google.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.4</a></li>
	  </ul>
	</li>
	<li><a href="http://www.google.com">Folder 1</a>
	  <ul class="multicolumn">
	  <li><a href="http://www.google.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.5</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.6</a></li>
	  <li><a href="http://www.google.com">Sub Item 1.7</a></li>
	  </ul>
	</li>
	<li><a href="http://www.google.com">Item 3</a></li>
	<li><a href="http://www.google.com">Folder 2</a>
	  <ul>
	  <li><a href="http://www.google.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.google.com">Sub Item 2.1</a></li>
	  </ul>
	</li>
	<li><a href="http://www.google.com/style/">Item 4</a></li>
	<li id="search">
		<form id="topform" method="get" action="http://www.google.com/search/search.php">
		<input type="text" name="zoom_query" id="zoom_query" size="20" class="zoom_searchbox topsearchbox" placeholder="search">
		<input id="query_submit" type="image" src="assets/magnify.gif" />
		<input name="zoom_per_page" id="zoom_per_page" type="hidden" value="10" />
		<input name="zoom_and" id="zoom_and" type="hidden" value="1" />
		<input type="hidden" name="zoom_sort" value="0" />
		</form>
	</li>
	</ul>
	
	</div>

## Configuring the "responsive" aspect of the menu ##

eFluidmenu is set up with 3 breaking points using CSS media queries by default. This can be seen at the bottom of "efluidmenu.css":

+ When the device/browser width is 1100px or below, the "#sitelogo" element shrinks from 55px to 40px.
+ When the device/browser width is 930px or below, the "#search" element is hidden.
+ When the device/browser width is 450px or below, the menu switches to the mobile menu version, with the main UL element hidden by default and toggle-able using the now visible "hamburger" menu link.

You'll most likely want to configure some or all aspects of the settings above depending on how many menu headers you have.

## Two ways to add a multi-column sub menu ##

eFluidmenu currently only supports one level deep of sub menus, though it makes up for this short coming by supporting multi-column sub menus. You can turn a regular UL nested menu into multiple columns, or specify an arbitrary DIV on the page as the sub menu, allowing for much more flexibility in what's shown inside the sub menu. See the page [Two ways to add a multi-column sub menu](http://dynamicdrive.com/dynamicindex1/efluidmenu/suppliment.htm) for details on both methods of adding a multi-column sub menu.


## More info ##

Visit the script's project page for additional details on setup and documentation: <http://dynamicdrive.com/dynamicindex1/efluidmenu/>
