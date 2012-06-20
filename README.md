#Description:
The aim of this test is to have a grid of items using media queries to change the number of items displayed per row depending on the available screen space. Using floats was not an option, since we have to support items of various lengths. Here is an [online test case](http://www.g-rom.be/reflowing_grid/).

* Uses display:inline-block; and media queries
* Reflows depending on the available width (4 items per row > 3 items per row > 2 items per row)
* Plays nice with items of various lengths
* Alleviates [the whitespace bug between items](http://css-tricks.com/fighting-the-space-between-inline-block-elements/). If you really want to be on the safe side here, use HTML comments to eliminate whitespace or block your begin and end tags together.
* Tested in all modern browsers and in IE >= 7 (slight float drops in IE7 upon window resize caused by sub-pixel rounding but I can live with that)
* Uses [selectivizr.js](https://github.com/keithclark/selectivizr) and [respond.js](https://github.com/scottjehl/Respond) to get support for CSS3 selectors and screen-size based media-queries in IE >=7