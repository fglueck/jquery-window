# jquery-window

```html
<!-- Style Includes -->
<link type="text/css" href="js/jquery/themes/black-tie/jquery-ui.css" rel="stylesheet" />
<link type="text/css" href="js/jquery/window/css/jquery.window.css" rel="stylesheet" />

<!-- JavaScript Includes -->
<script type="text/javascript" src="js/jquery/jquery.js"></script>
<script type="text/javascript" src="js/jquery/jquery-ui.js"></script>
<script type="text/javascript" src="js/jquery/window/jquery.window.js"></script>
```

```javascript
$.window({
	title: 'SQL Server Reporting Services Schulung'
  , url: 'http://www.dozent.net/Schulung/Datenbank/MS-SQL-Server/152/'
});

Catch the Window inside a div
$('#div').window({
	title: 'PostgreSQL Schulung'
  , url: 'http://www.dozent.net/Schulung/Datenbank/PostgreSQL/'
})
```


## Static Attributes

<table>
	<tr>
		<td>dock</td>
		<td><span>[string:"left"]</span> the direction of minimized
			window dock at. the available values are [left, right, top, bottom]</td>
	</tr>
	<tr>
		<td>dockArea</td>
		<td><span>[jquery object, element:null]</span> the area which the
			windows will dock at</td>
	</tr>
	<tr>
		<td>animationSpeed</td>
		<td><span>[number:400]</span> the speed of animations: maximize,
			minimize, restore, shift, in milliseconds</td>
	</tr>
	<tr>
		<td>minWinNarrow</td>
		<td><span>[number:24]</span> the narrow dimension of minimized
			window</td>
	</tr>
	<tr>
		<td>minWinLong</td>
		<td><span>[number:120]</span> the long dimension of minimized
			window</td>
	</tr>
	<tr>
		<td>handleScrollbar</td>
		<td><span>[boolean:true]</span> to handle browser scrollbar when
			window status changed(maximize, minimize, cascade)</td>
	</tr>
	<tr>
		<td>showLog</td>
		<td><span>[boolean:false]</span> to decide show log in firebug,
			IE8, chrome console</td>
	</tr>
</table>

## Instance Attributes


<table>
	<tr>
		<td>icon</td>
		<td><span>[string:"auto"]</span> an icon image url string. if
			this attribute is given, it will force to replace the original
			favicon of remote page on window. or you can set it as null to hide
			icon.</td>
	</tr>
	<tr>
		<td>title</td>
		<td><span>[string:""]</span> the title text of window</td>
	</tr>
	<tr>
		<td>url</td>
		<td><span>[string:""]</span> the target url of iframe ready to
			load.</td>
	</tr>
	<tr>
		<td>content</td>
		<td><span>[html string, jquery object, element:""]</span> this
			attribute only works when url is null. when passing a jquery object
			or a element, it will clone the original one to append.</td>
	</tr>
	<tr>
		<td>footerContent</td>
		<td><span>[html string, jquery object, element:""]</span> same as
			content attribute, but it's put on footer panel.</td>
	</tr>
	<tr>
		<td>containerClass</td>
		<td><span>[string:""]</span> container extra class</td>
	</tr>
	<tr>
		<td>headerClass</td>
		<td><span>[string:""]</span> header extra class</td>
	</tr>
	<tr>
		<td>frameClass</td>
		<td><span>[string:""]</span> frame extra class</td>
	</tr>
	<tr>
		<td>footerClass</td>
		<td><span>[string:""]</span> footer extra class</td>
	</tr>
	<tr>
		<td>selectedHeaderClass</td>
		<td><span>[string:""]</span> selected header extra class</td>
	</tr>
	<tr>
		<td>x</td>
		<td><span>[number:-1]</span> the x-axis value on screen(or caller
			element), if -1 means put on screen(or caller element) center</td>
	</tr>
	<tr>
		<td>y</td>
		<td><span>[number:-1]</span> the y-axis value on screen(or caller
			element), if -1 means put on screen(or caller element) center</td>
	</tr>
	<tr>
		<td>z</td>
		<td><span>[number:2000]</span> the css z-index value</td>
	</tr>
	<tr>
		<td>width</td>
		<td><span>[number:400]</span> window width</td>
	</tr>
	<tr>
		<td>height</td>
		<td><span>[number:300]</span> window height</td>
	</tr>
	<tr>
		<td>minWidth</td>
		<td><span>[number:200]</span> the minimum width, if -1 means no
			checking</td>
	</tr>
	<tr>
		<td>minHeight</td>
		<td><span>[number:150]</span> the minimum height, if -1 means no
			checking</td>
	</tr>
	<tr>
		<td>maxWidth</td>
		<td><span>[number:800]</span> the maximum width, if -1 means no
			checking</td>
	</tr>
	<tr>
		<td>maxHeight</td>
		<td><span>[number:600]</span> the maximum height, if -1 means no
			checking</td>
	</tr>
	<tr>
		<td>showModal</td>
		<td><span>[boolean:false]</span> to control show modal on
			background</td>
	</tr>
	<tr>
		<td>modalOpacity</td>
		<td><span>[number:0.5]</span> the opacity of modal dialog</td>
	</tr>
	<tr>
		<td>showFooter</td>
		<td><span>[boolean:true]</span> to control show footer panel</td>
	</tr>
	<tr>
		<td>showRoundCorner</td>
		<td><span>[boolean:true]</span> to control display window as
			round corner</td>
	</tr>
	<tr>
		<td>closable</td>
		<td><span>[boolean:true]</span> to control window closable</td>
	</tr>
	<tr>
		<td>minimizable</td>
		<td><span>[boolean:true]</span> to control window minimizable</td>
	</tr>
	<tr>
		<td>maximizable</td>
		<td><span>[boolean:true]</span> to control window maximizable</td>
	</tr>
	<tr>
		<td>bookmarkable</td>
		<td><span>[boolean:true]</span> to control window with remote url
			could be bookmarked</td>
	</tr>
	<tr>
		<td>draggable</td>
		<td><span>[boolean:true]</span> to control window draggable</td>
	</tr>
	<tr>
		<td>resizable</td>
		<td><span>[boolean:true]</span> to control window resizable</td>
	</tr>
	<tr>
		<td>scrollable</td>
		<td><span>[boolean:true]</span> to show scroll bar or not</td>
	</tr>
	<tr>
		<td>checkBoundary</td>
		<td><span>[boolean:false]</span> to check window dialog overflow
			html body or caller element</td>
	</tr>
	<tr>
		<td>withinBrowserWindow</td>
		<td><span>[boolean:false]</span> to limit window only can be
			dragged within browser window. this attribute only works when
			checkBoundary is true and caller is null.</td>
	</tr>
	<tr>
		<td>custBtns</td>
		<td><span>[json array:null]</span> to describe the customized
			button display and callback function</td>
	</tr>
	<tr>
		<td>onOpen</td>
		<td><span>[function:null]</span> a callback function while
			container is added into body</td>
	</tr>
	<tr>
		<td>onShow</td>
		<td><span>[function:null]</span> a callback function while whole
			window display routine is finished</td>
	</tr>
	<tr>
		<td>onClose</td>
		<td><span>[function:null]</span> a callback function while user
			click close button</td>
	</tr>
	<tr>
		<td>onSelect</td>
		<td><span>[function:null]</span> a callback function while user
			select the window</td>
	</tr>
	<tr>
		<td>onUnselect</td>
		<td><span>[function:null]</span> a callback function while window
			unselected</td>
	</tr>
	<tr>
		<td>onDrag</td>
		<td><span>[function:null]</span> a callback function while window
			is going to drag</td>
	</tr>
	<tr>
		<td>afterDrag</td>
		<td><span>[function:null]</span> a callback function after window
			dragged</td>
	</tr>
	<tr>
		<td>onResize</td>
		<td><span>[function:null]</span> a callback function while window
			is going to resize</td>
	</tr>
	<tr>
		<td>afterResize</td>
		<td><span>[function:null]</span> a callback function after window
			resized</td>
	</tr>
	<tr>
		<td>onMinimize</td>
		<td><span>[function:null]</span> a callback function while window
			is going to minimize</td>
	</tr>
	<tr>
		<td>afterMinimize</td>
		<td><span>[function:null]</span> a callback function after window
			minimized</td>
	</tr>
	<tr>
		<td>onMaximize</td>
		<td><span>[function:null]</span> a callback function while window
			is going to maximize</td>
	</tr>
	<tr>
		<td>afterMaximize</td>
		<td><span>[function:null]</span> a callback function after window
			maximized</td>
	</tr>
	<tr>
		<td>onCascade</td>
		<td><span>[function:null]</span> a callback function while window
			is going to cascade</td>
	</tr>
	<tr>
		<td>afterCascade</td>
		<td><span>[function:null]</span> a callback function after window
			cascaded</td>
	</tr>
	<tr>
		<td>onIframeStart</td>
		<td><span>[function:null]</span> a callback function while iframe
			ready to connect remoting url. this attribute only works while url
			attribute is given</td>
	</tr>
	<tr>
		<td>onIframeEnd</td>
		<td><span>[function:null]</span> a callback function while iframe
			load finished. this attribute only works while url attribute is given</td>
	</tr>
	<tr>
		<td>iframeRedirectCheckMsg</td>
		<td><span>[string:null]</span> if null means no check, or pass a
			string to show warning message while iframe is going to redirect
			current top page</td>
	</tr>
	<tr>
		<td>createRandomOffset</td>
		<td><span>[json object:{x:0, y:0}]</span> random the new created
			window position, it only works when options x,y value both are -1</td>
	</tr>
</table>
	   
## Static Methods ( $.window.[method name] )

<table>
	<tr>
		<td>prepare</td>
		<td>initialize with customerized static setting attributes</td>
	</tr>
	<tr>
		<td><font color="#000">∟</font> custSetting</td>
		<td><span>[object]</span>the customerized static attributes
			object</td>
	</tr>
	<tr>
		<td>closeAll</td>
		<td>close all created windows</td>
	</tr>
	<tr>
		<td><font color="#000">∟</font> quiet</td>
		<td><span>[boolean]</span>to decide doing callback or not</td>
	</tr>
	<tr>
		<td>hideAll</td>
		<td>hide all created windows</td>
	</tr>
	<tr>
		<td>showAll</td>
		<td>show all created windows</td>
	</tr>
	<tr>
		<td>getAll</td>
		<td>return all created windows instance</td>
	</tr>
	<tr>
		<td>getWindow</td>
		<td>get the window instance by passed window id</td>
	</tr>
	<tr>
		<td><font color="#000">∟</font> windowId</td>
		<td><span>[string]</span>the target window id</td>
	</tr>
	<tr>
		<td>getSelectedWindow</td>
		<td>get the selected window instance</td>
	</tr>
</table>
			
## Instance Methods			

<table>
	<tr>
		<td>getWindowId</td>
		<td>get window id</td>
	</tr>
	<tr>
		<td>getCaller</td>
		<td>get window container's parent panel, it's a jQuery object</td>
	</tr>
	<tr>
		<td>getContainer</td>
		<td>get window container panel, it's a jQuery object</td>
	</tr>
	<tr>
		<td>getHeader</td>
		<td>get window header panel, it's a jQuery object</td>
	</tr>
	<tr>
		<td>getFrame</td>
		<td>get window frame panel, it's a jQuery object</td>
	</tr>
	<tr>
		<td>getFooter</td>
		<td>get window footer panel, it's a jQuery object</td>
	</tr>
	<tr>
		<td>alignCenter</td>
		<td>set current window as screen center</td>
	</tr>
	<tr>
		<td>alignHorizontalCenter</td>
		<td>set current window as horizontal center</td>
	</tr>
	<tr>
		<td>alignVerticalCenter</td>
		<td>set current window as vertical center</td>
	</tr>
	<tr>
		<td>select</td>
		<td>select current window, it will increase the original z-index
			value with 2</td>
	</tr>
	<tr>
		<td>unselect</td>
		<td>unselect current window, it will set the z-index as original
			options.z</td>
	</tr>
	<tr>
		<td>move</td>
		<td>move current window to target position or shift it by passed
			distance</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> x</td>
		<td><span>[number]</span>the absolute x-axis value on document or
			shift distance, in pixels</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> y</td>
		<td><span>[number]</span>the absolute y-axis value on document or
			shift distance, in pixels</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> bShift</td>
		<td><span>[boolean]</span>a boolean flag to decide to shift the
			window position with x,y</td>
	</tr>
	<tr>
		<td>resize</td>
		<td>resize current window to target width/height</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> w</td>
		<td><span>[number]</span>target width value, in pixels</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> h</td>
		<td><span>[number]</span>target height value, in pixels</td>
	</tr>
	<tr>
		<td>maximize</td>
		<td>maximize current window</td>
	</tr>
	<tr>
		<td>minimize</td>
		<td>minimize current window</td>
	</tr>
	<tr>
		<td>restore</td>
		<td>restore current window, it could be maximized or cascade
			status</td>
	</tr>
	<tr>
		<td>close</td>
		<td>close current window</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> quiet</td>
		<td><span>[boolean]</span>to decide doing callback or not</td>
	</tr>
	<tr>
		<td>hide</td>
		<td>hide current window</td>
	</tr>
	<tr>
		<td>show</td>
		<td>show current window</td>
	</tr>
	<tr>
		<td>setTitle</td>
		<td>change window title</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> title</td>
		<td><span>[string]</span>window title text</td>
	</tr>
	<tr>
		<td>setUrl</td>
		<td>change iframe url</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> url</td>
		<td><span>[string]</span>iframe url</td>
	</tr>
	<tr>
		<td>setContent</td>
		<td>change frame content</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> content</td>
		<td><span>[html string, jquery object, element]</span> the
			content of frame</td>
	</tr>
	<tr>
		<td>setFooterContent</td>
		<td>change footer content</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> content</td>
		<td><span>[html string, jquery object, element]</span> the
			content of footer</td>
	</tr>
	<tr>
		<td>getTitle</td>
		<td>get window title text</td>
	</tr>
	<tr>
		<td>getUrl</td>
		<td>get url string</td>
	</tr>
	<tr>
		<td>getContent</td>
		<td>get frame html content</td>
	</tr>
	<tr>
		<td>getFooterContent</td>
		<td>get footer html content</td>
	</tr>
	<tr>
		<td>isMaximized</td>
		<td>get window maximized status</td>
	</tr>
	<tr>
		<td>isMinimized</td>
		<td>get window minmized status</td>
	</tr>
	<tr>
		<td>isSelected</td>
		<td>get window selected status</td>
	</tr>
	<tr>
		<td>setIcon</td>
		<td>set window icon</td>
	</tr>
	<tr>
		<td><font color="#000">?</font> iconUrl</td>
		<td><span>[string]</span> the image url of icon</td>
	</tr>
	<tr>
		<td>showIcon</td>
		<td>show window icon</td>
	</tr>
	<tr>
		<td>hideIcon</td>
		<td>hide window icon</td>
	</tr>
</table>

		