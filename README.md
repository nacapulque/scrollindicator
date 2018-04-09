# scrollindicator

## code from deleted bower dependency @charaplessa

scrollindicator.js is a jQuery plugin that adds a bar on your page, which indicates the percentage of the page that has been scrolled.

## Depedencies
This is a jQuery plugin, so jQuery must be imported to your project prior scrollindicator.js script.

## Installation

##### Normal installation
Just copy the js/scrollindicator.js file into your project. Don't forget to also include dependecy files into your project.
```
<script src="jquery.js"></script>
<script src="scrollindicator.js"></script>
```
<br>
<br>
#####Bower installation
Just type the following command:
```
bower install scrollindicator
```

## Initialization

To initialize the plugin add the following JavaScript code into your project:
```
(function($) {
    'use strict';
     
     $(document).ready(function() {
         
         $('body').scrollindicator();

     });
     
})(jQuery);
```

This plugin provides you some optional options which you can use to achieve customization. The options are presented below.
For instance:
```
$('body').scrollindicator({ 
            backgroundColor: 'transparent',
            color: 'black',
            gradientFinish: 'yellow',
            where: 'header',
            position: 'top',
            width: '5px'
 });
```


## Manual
Plugin options are:

##### backgroundColor
Behind the bar color. If omitted the default is transparent.

##### color
Bar's color.

##### gradientFinish
If set, the bar has a gradient color and color option is used for gradientStart.
If both color and gradientFinish options are omitted, bar has a gradient blue color.

##### where
Bar's position, eg: 'header' to be placed in < header >, or '#myheader' to be placed in $('#myheader').
If omitted, the bar by default is placed with fixed position, at the top or at the bottom of the page, according to position option.


##### position
Top or bottom, if top, the bar is placed at the top of $(where), if bottom, bar is placed at the bottom of $(where).
If omitted, the default is top.

##### width
Bar's width. If omitted, width is set to 5px by default.

Enjoy the script and let me know for any suggestions you may have for further enhancement!

Cheers!
