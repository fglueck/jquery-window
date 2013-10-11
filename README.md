jquery-window
=============
<!-- Style Includes -->
<link type="text/css" href="js/jquery/themes/black-tie/jquery-ui.css" rel="stylesheet" />
<link type="text/css" href="js/jquery/window/css/jquery.window.css" rel="stylesheet" />

<!-- JavaScript Includes -->
<script type="text/javascript" src="js/jquery/jquery.js"></script>
<script type="text/javascript" src="js/jquery/jquery-ui.js"></script>
<script type="text/javascript" src="js/jquery/window/jquery.window.js"></script>


$.window({
	title: 'SQL Server Reporting Services Schulung'
  , url: 'http://www.dozent.net/Schulung/Datenbank/MS-SQL-Server/152/'
});

Catch the Window inside a div
$('#div').window({
	title: 'PostgreSQL Schulung'
  , url: 'http://www.dozent.net/Schulung/Datenbank/PostgreSQL/'
})

<div class="readme_block" id="attributes_block">
			<h3>Static Attributes</h3>
			<table class="attributes_list">
				<tbody><tr><td class="attribute">dock</td>
					<td class="attr_desc"><span class="format_define">[string:"left"]</span> the direction of minimized window dock at. the available values are [left, right, top, bottom]</td>
				</tr>
				<tr><td class="attribute">dockArea</td>
					<td class="attr_desc"><span class="format_define">[jquery object, element:null]</span> the area which the windows will dock at</td>
				</tr>
				<tr><td class="attribute">animationSpeed</td>
					<td class="attr_desc"><span class="format_define">[number:400]</span> the speed of animations: maximize, minimize, restore, shift, in milliseconds</td>
				</tr>
				<tr><td class="attribute">minWinNarrow</td>
					<td class="attr_desc"><span class="format_define">[number:24]</span> the narrow dimension of minimized window</td>
				</tr>
				<tr><td class="attribute">minWinLong</td>
					<td class="attr_desc"><span class="format_define">[number:120]</span> the long dimension of minimized window</td>
				</tr>
				<tr><td class="attribute">handleScrollbar</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to handle browser scrollbar when window status changed(maximize, minimize, cascade)</td>
				</tr>
				<tr><td class="attribute">showLog</td>
					<td class="attr_desc"><span class="format_define">[boolean:false]</span> to decide show log in firebug, IE8, chrome console</td>
				</tr>
			</tbody></table>
			<br>
			
			<h3>Instance Attributes</h3>
			<table class="attributes_list">
				<tbody><tr><td class="attribute">icon</td>
					<td class="attr_desc"><span class="format_define">[string:"auto"]</span> an icon image url string. if this attribute is given, it will force to replace the original favicon of remote page on window. or you can set it as null to hide icon.</td>
				</tr>
				<tr><td class="attribute">title</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> the title text of window</td>
				</tr>
				<tr><td class="attribute">url</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> the target url of iframe ready to load.</td>
				</tr>
				<tr><td class="attribute">content</td>
					<td class="attr_desc"><span class="format_define">[html string, jquery object, element:""]</span> this attribute only works when url is null. when passing a jquery object or a element, it will clone the original one to append.</td>
				</tr>
				<tr><td class="attribute">footerContent</td>
					<td class="attr_desc"><span class="format_define">[html string, jquery object, element:""]</span> same as content attribute, but it's put on footer panel.</td>
				</tr>
				<tr><td class="attribute">containerClass</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> container extra class</td>
				</tr>
				<tr><td class="attribute">headerClass</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> header extra class</td>
				</tr>
				<tr><td class="attribute">frameClass</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> frame extra class</td>
				</tr>
				<tr><td class="attribute">footerClass</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> footer extra class</td>
				</tr>
				<tr><td class="attribute">selectedHeaderClass</td>
					<td class="attr_desc"><span class="format_define">[string:""]</span> selected header extra class</td>
				</tr>
				<tr><td class="attribute">x</td>
					<td class="attr_desc"><span class="format_define">[number:-1]</span> the x-axis value on screen(or caller element), if -1 means put on screen(or caller element) center</td>
				</tr>
				<tr><td class="attribute">y</td>
					<td class="attr_desc"><span class="format_define">[number:-1]</span> the y-axis value on screen(or caller element), if -1 means put on screen(or caller element) center</td>
				</tr>
				<tr><td class="attribute">z</td>
					<td class="attr_desc"><span class="format_define">[number:2000]</span> the css z-index value</td>
				</tr>
				<tr><td class="attribute">width</td>
					<td class="attr_desc"><span class="format_define">[number:400]</span> window width</td>
				</tr>
				<tr><td class="attribute">height</td>
					<td class="attr_desc"><span class="format_define">[number:300]</span> window height</td>
				</tr>
				<tr><td class="attribute">minWidth</td>
					<td class="attr_desc"><span class="format_define">[number:200]</span> the minimum width, if -1 means no checking</td>
				</tr>
				<tr><td class="attribute">minHeight</td>
					<td class="attr_desc"><span class="format_define">[number:150]</span> the minimum height, if -1 means no checking</td>
				</tr>
				<tr><td class="attribute">maxWidth</td>
					<td class="attr_desc"><span class="format_define">[number:800]</span> the maximum width, if -1 means no checking</td>
				</tr>
				<tr><td class="attribute">maxHeight</td>
					<td class="attr_desc"><span class="format_define">[number:600]</span> the maximum height, if -1 means no checking</td>
				</tr>
				<tr><td class="attribute">showModal</td>
					<td class="attr_desc"><span class="format_define">[boolean:false]</span> to control show modal on background</td>
				</tr>
				<tr><td class="attribute">modalOpacity</td>
					<td class="attr_desc"><span class="format_define">[number:0.5]</span> the opacity of modal dialog</td>
				</tr>
				<tr><td class="attribute">showFooter</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control show footer panel</td>
				</tr>
				<tr><td class="attribute">showRoundCorner</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control display window as round corner</td>
				</tr>
				<tr><td class="attribute">closable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window closable</td>
				</tr>
				<tr><td class="attribute">minimizable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window minimizable</td>
				</tr>
				<tr><td class="attribute">maximizable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window maximizable</td>
				</tr>
				<tr><td class="attribute">bookmarkable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window with remote url could be bookmarked</td>
				</tr>
				<tr><td class="attribute">draggable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window draggable</td>
				</tr>
				<tr><td class="attribute">resizable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to control window resizable</td>
				</tr>
				<tr><td class="attribute">scrollable</td>
					<td class="attr_desc"><span class="format_define">[boolean:true]</span> to show scroll bar or not</td>
				</tr>
				<tr><td class="attribute">checkBoundary</td>
					<td class="attr_desc"><span class="format_define">[boolean:false]</span> to check window dialog overflow html body or caller element</td>
				</tr>
				<tr><td class="attribute">withinBrowserWindow</td>
					<td class="attr_desc"><span class="format_define">[boolean:false]</span> to limit window only can be dragged within browser window. this attribute only works when checkBoundary is true and caller is null.</td>
				</tr>
				<tr><td class="attribute">custBtns</td>
					<td class="attr_desc"><span class="format_define">[json array:null]</span> to describe the customized button display and callback function</td>
				</tr>
				<tr><td class="attribute">onOpen</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while container is added into body</td>
				</tr>
				<tr><td class="attribute">onShow</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while whole window display routine is finished</td>
				</tr>
				<tr><td class="attribute">onClose</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while user click close button</td>
				</tr>
				<tr><td class="attribute">onSelect</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while user select the window</td>
				</tr>
				<tr><td class="attribute">onUnselect</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window unselected</td>
				</tr>
				<tr><td class="attribute">onDrag</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window is going to drag</td>
				</tr>
				<tr><td class="attribute">afterDrag</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function after window dragged</td>
				</tr>
				<tr><td class="attribute">onResize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window is going to resize</td>
				</tr>
				<tr><td class="attribute">afterResize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function after window resized</td>
				</tr>
				<tr><td class="attribute">onMinimize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window is going to minimize</td>
				</tr>
				<tr><td class="attribute">afterMinimize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function after window minimized</td>
				</tr>
				<tr><td class="attribute">onMaximize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window is going to maximize</td>
				</tr>
				<tr><td class="attribute">afterMaximize</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function after window maximized</td>
				</tr>
				<tr><td class="attribute">onCascade</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while window is going to cascade</td>
				</tr>
				<tr><td class="attribute">afterCascade</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function after window cascaded</td>
				</tr>
				<tr><td class="attribute">onIframeStart</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while iframe ready to connect remoting url. this attribute only works while url attribute is given</td>
				</tr>
				<tr><td class="attribute">onIframeEnd</td>
					<td class="attr_desc"><span class="format_define">[function:null]</span> a callback function while iframe load finished. this attribute only works while url attribute is given</td>
				</tr>
				<tr><td class="attribute">iframeRedirectCheckMsg</td>
					<td class="attr_desc"><span class="format_define">[string:null]</span> if null means no check, or pass a string to show warning message while iframe is going to redirect current top page</td>
				</tr>
				<tr><td class="attribute">createRandomOffset</td>
					<td class="attr_desc"><span class="format_define">[json object:{x:0, y:0}]</span> random the new created window position, it only works when options x,y value both are -1</td>
				</tr>
			</tbody></table>
		</div>
		
		<div class="readme_block" id="methods_block">
			<h3>Static Methods ( $.window.[method name] )</h3>
			<table class="methods_list">
				<tbody><tr><td class="method_name">prepare</td>
					<td class="method_desc">initialize with customerized static setting attributes</td>
				</tr>
					<tr><td class="method_param"><font color="#000">∟</font> custSetting</td>
						<td class="method_desc"><span class="format_define">[object]</span>the customerized static attributes object</td>
					</tr>
				<tr><td class="method_name">closeAll</td>
					<td class="method_desc">close all created windows</td>
				</tr>
					<tr><td class="method_param"><font color="#000">∟</font> quiet</td>
						<td class="method_desc"><span class="format_define">[boolean]</span>to decide doing callback or not</td>
					</tr>
				<tr><td class="method_name">hideAll</td>
					<td class="method_desc">hide all created windows</td>
				</tr>
				<tr><td class="method_name">showAll</td>
					<td class="method_desc">show all created windows</td>
				</tr>
				<tr><td class="method_name">getAll</td>
					<td class="method_desc">return all created windows instance</td>
				</tr>
				<tr><td class="method_name">getWindow</td>
					<td class="method_desc">get the window instance by passed window id</td>
				</tr>
					<tr><td class="method_param"><font color="#000">∟</font> windowId</td>
						<td class="method_desc"><span class="format_define">[string]</span>the target window id</td>
					</tr>
				<tr><td class="method_name">getSelectedWindow</td>
					<td class="method_desc">get the selected window instance</td>
				</tr>
			</tbody></table>
			<br>
			
			<h3>Instance Methods</h3>
			<table class="methods_list">
				<tbody><tr><td class="method_name">getWindowId</td>
					<td class="method_desc">get window id</td>
				</tr>
				<tr><td class="method_name">getCaller</td>
					<td class="method_desc">get window container's parent panel, it's a jQuery object</td>
				</tr>
				<tr><td class="method_name">getContainer</td>
					<td class="method_desc">get window container panel, it's a jQuery object</td>
				</tr>
				<tr><td class="method_name">getHeader</td>
					<td class="method_desc">get window header panel, it's a jQuery object</td>
				</tr>
				<tr><td class="method_name">getFrame</td>
					<td class="method_desc">get window frame panel, it's a jQuery object</td>
				</tr>
				<tr><td class="method_name">getFooter</td>
					<td class="method_desc">get window footer panel, it's a jQuery object</td>
				</tr>
				<tr><td class="method_name">alignCenter</td>
					<td class="method_desc">set current window as screen center</td>
				</tr>
				<tr><td class="method_name">alignHorizontalCenter</td>
					<td class="method_desc">set current window as horizontal center</td>
				</tr>
				<tr><td class="method_name">alignVerticalCenter</td>
					<td class="method_desc">set current window as vertical center</td>
				</tr>
				<tr><td class="method_name">select</td>
					<td class="method_desc">select current window, it will increase the original z-index value with 2</td>
				</tr>
				<tr><td class="method_name">unselect</td>
					<td class="method_desc">unselect current window, it will set the z-index as original options.z</td>
				</tr>
				<tr><td class="method_name">move</td>
					<td class="method_desc">move current window to target position or shift it by passed distance</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> x</td>
					<td class="method_desc"><span class="format_define">[number]</span>the absolute x-axis value on document or shift distance, in pixels</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> y</td>
					<td class="method_desc"><span class="format_define">[number]</span>the absolute y-axis value on document or shift distance, in pixels</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> bShift</td>
					<td class="method_desc"><span class="format_define">[boolean]</span>a boolean flag to decide to shift the window position with x,y</td>
				</tr>
				<tr><td class="method_name">resize</td>
					<td class="method_desc">resize current window to target width/height</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> w</td>
					<td class="method_desc"><span class="format_define">[number]</span>target width value, in pixels</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> h</td>
					<td class="method_desc"><span class="format_define">[number]</span>target height value, in pixels</td>
				</tr>
				<tr><td class="method_name">maximize</td>
					<td class="method_desc">maximize current window</td>
				</tr>
				<tr><td class="method_name">minimize</td>
					<td class="method_desc">minimize current window</td>
				</tr>
				<tr><td class="method_name">restore</td>
					<td class="method_desc">restore current window, it could be maximized or cascade status</td>
				</tr>
				<tr><td class="method_name">close</td>
					<td class="method_desc">close current window</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> quiet</td>
					<td class="method_desc"><span class="format_define">[boolean]</span>to decide doing callback or not</td>
				</tr>
				<tr><td class="method_name">hide</td>
					<td class="method_desc">hide current window</td>
				</tr>
				<tr><td class="method_name">show</td>
					<td class="method_desc">show current window</td>
				</tr>
				<tr><td class="method_name">setTitle</td>
					<td class="method_desc">change window title</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> title</td>
					<td class="method_desc"><span class="format_define">[string]</span>window title text</td>
				</tr>
				<tr><td class="method_name">setUrl</td>
					<td class="method_desc">change iframe url</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> url</td>
					<td class="method_desc"><span class="format_define">[string]</span>iframe url</td>
				</tr>
				<tr><td class="method_name">setContent</td>
					<td class="method_desc">change frame content</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> content</td>
					<td class="method_desc"><span class="format_define">[html string, jquery object, element]</span> the content of frame</td>
				</tr>
				<tr><td class="method_name">setFooterContent</td>
					<td class="method_desc">change footer content</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> content</td>
					<td class="method_desc"><span class="format_define">[html string, jquery object, element]</span> the content of footer</td>
				</tr>
				<tr><td class="method_name">getTitle</td>
					<td class="method_desc">get window title text</td>
				</tr>
				<tr><td class="method_name">getUrl</td>
					<td class="method_desc">get url string</td>
				</tr>
				<tr><td class="method_name">getContent</td>
					<td class="method_desc">get frame html content</td>
				</tr>
				<tr><td class="method_name">getFooterContent</td>
					<td class="method_desc"> get footer html content</td>
				</tr>
				<tr><td class="method_name">isMaximized</td>
					<td class="method_desc">get window maximized status</td>
				</tr>
				<tr><td class="method_name">isMinimized</td>
					<td class="method_desc">get window minmized status</td>
				</tr>
				<tr><td class="method_name">isSelected</td>
					<td class="method_desc">get window selected status</td>
				</tr>
				<tr><td class="method_name">setIcon</td>
					<td class="method_desc">set window icon</td>
				</tr>
				<tr><td class="method_param"><font color="#000">∟</font> iconUrl</td>
					<td class="method_desc"><span class="format_define">[string]</span> the image url of icon</td>
				</tr>
				<tr><td class="method_name">showIcon</td>
					<td class="method_desc">show window icon</td>
				</tr>
				<tr><td class="method_name">hideIcon</td>
					<td class="method_desc">hide window icon</td>
				</tr>
			</tbody></table>
		</div>