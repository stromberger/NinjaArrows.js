NinjaArrows.js
==============

A Google Maps/OpenLayers extension that shows small arrows at the map's egeds indicating out of bounds markers.

Usage
-----

**Google Maps**
To use NinjaArrows and its features simply create a new NinjaArrows instance by passing a valid map to the constructor.
```javascript
var ninjaArrows = new NinjaArrows(map);
```

You can also pass an existing array of Markers to the constructor:
```javascript
var markers = [];

// add markers ...

var ninjaArrows = new NinjaArrows(map, markers);
```

You can alos instantiate NinjaArrows with several options, i.e. style, offsets etc.
```javascript
var customStyle = {
  fillColor: "yellow",
  strokeColor: "orange",
  strokeWidth: 2,
  textColor: "black"
};
var ninjaArrows = new NinjaArrows(map, markers, { style: customStyle );
```

To add a new marker simply call addMarker():
```javascript
ninjaArrows.addMarker(marker);
```

The same applies to removing markers. Just call removeMarker() to remove the given marker from NinjaArrows. 
```javascript
ninjaArrows.removeMarker(marker);
```

To clear all markers, call clearMarkers():
```javascript
ninjaArrows.clearMarkers();
```

To show and hide the arrows call show()/hide():
```javascript
ninjaArrows.show();

ninjaArrows.hide();
```


**OpenLayers**
OpenLayers version comming soon ;)
