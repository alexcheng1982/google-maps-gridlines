Google Maps Gridlines
=====================

This is a small JavaScript file to create latitude/longitude gridlines over Google Maps. 

The original version was made by [Bill Chadwick](http://www.bdcc.co.uk/Gmaps/BdccGmapBits.htm) and then other contributors continued to improve it. Refer to the file's comment for more information. 

I made some improvements and made this library available in Bower. 

* Fix JSHint errors.
* Fix the issue that this library causes map to freeze in Chrome/Safari on Mac.

### Install

Use `bower install google-maps-gridlines` to install using Bower.


### How to use

To show gridlines on Google map, use code like this

```
var mapOptions = {
	center: new google.maps.LatLng(-42, 174),
	zoom: 5
};
var map = new google.maps.Map(document.getElementById("map-canvas"), mapOptions);
var gridlines = new Graticule(map);
```

### Sample Page

To view example usage, check out `test/simple-map.html` page. You can start a simple HTTP server using `python -m SimpleHTTPServer` and view this sample page.