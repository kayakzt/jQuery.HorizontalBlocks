#jQuery HorizontalBlocks v1.2 -
jQuery Horizonal Blocks can change your website to scrollable horizontal blocks easily.  
  
Open source under the BSD License.  
Copyright 2013 Kakurezatou <[http://kakurezatou.com/](http://kakurezatou.com/)>  
All rights reserved.  
  
*[Demo Page](http://kakurezatou.com/software/jqueryplugin/HorizontalBlocks/)*
##How to use
Loading jQuery and Horizonal Blocks,  
```html
<script src="jquery.js" type="text/javascript"></script>
<script src="jquery.HorizontalBlocks.1.0.js" type="text/javascript"></script>
```
then write below html tags. It must be under the body tag.  
```html
<ul id="blocks">
    <li>Block1 Contents</li>
    <li>Block2 Contents</li>
    <li>Block2 Contents</li>
</ul>
<a id="nextBlock" href="#">Next</a>
<a id="prevBlock" href="#">Prev</a>
```
Finally, write below script.  
```javascript
$(document).HorizontalBlocks();  
```
##Options
Horizonal Blocks has some options. Default params are displayed below.  
```javascript
$(document).HorizontalBlocks({
    parentBox: "#box", //parent blocks tag
    block:"#blocks li", //blocks terget
    firstBlock: 1, // first displayed block number
    scrollOption:"swing", //set scroll type
    scrollSpeed: "normal", //set scroll speed.value(ms) or "normal", "slow", "fast"
    horizontalMenu: "nav a", // jump link terget
    nextId: "#nextBlock", //Id for Next Block
    prevId: "#prevBlock" //Id for Prev Block
});
```
If you loaded jQuery easing plugin, you could use more scroll option. 
jQuery easing plugin can download [here](http://gsgd.co.uk/sandbox/jquery/easing/).  
##revealed probrem
* collupse layout when access small display


##Release note
2013/02/23 Publish v1.2  
* fix scrolling performance on iOS and Android.  
* add swipe scrolling when access touch devices.  
  
2013/02/09 Publish v1.0  
