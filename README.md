﻿<span style=display:none; >[You are now in a GitHub source code view - click this link to view the home page]( http://ladybug-analysis-tools.github.io/ladybug-web/ "View file as a web page." ) </span>
<input type=button onclick=window.location.href='https://github.com/ladybug-analysis-tools/ladybug-web'; 
value='You are now in the home page view - Click this button to view the read me file and the source code' >

[Ladybug Analysis Tools]( https://github.com/ladybug-analysis-tools ) »


[Ladybug Web]( index.html )
===

_Ladybug for web provides solar and weather data visualization and analysis on the web_

Genarally the following scripts

* Built using entry level JavaScript with no dependencies other than Three.js and/or SunCalc.js


## [Analemma 3D]( http://ladybug-analysis-tools.github.io/ladybug-web/analemma-3d/ )


### Features

* 3D plot of analemmas of Sun azimuth and altitude once an hour for days 1 through 28 of each month. 
* Default latitude and longitude is San Francisco
* Sliders update latitude and longitude of analemma in real-time
* Displays map of location
	* Nine maps styles to choose from
* Buttons available for selected cities
* Midnight highlighted is red. Noon highlighted in green
* Placards indicate the hour of each analemma
* Permalink support
* Slide-out menu support

### Latest update: 2016-03-14 / R3

* Code clean-up

### Issues

* Has math error: noon and midnight analemmas are not opposite each other. 
	* Observe this error when viewing latitudes near Equator
* Map not positioning correctly


## [Analemma 2D]( http://ladybug-analysis-tools.github.io/ladybug-web/analemma-2d/ )

### Features

* 2D plot of Sun azimuth and altitude once an hour at the 21st of each month. 
* Default is lat/lon of San Francisco
* Latitude and longitude sliders - with real-time updates
* Buttons to display data for New York, Isfahan, San Francisco and Sydney
* Midnight highlighted in red. Noon highlighted in green
* Hourly data output in degrees
* Permalink support
* Slide-out menu support - helps with use on tablets

### Latest update: 2016-03-14 /R3

* Rename from 'Analemma Sandbox' to 'Analemma 2D'
* Adds slide-out 'hamburger' menu
* Code clean-up
* Adds latitude and longitude sliders - real-time updates
* Display and text readout calculated in degrees ( was radians ) 
* Permalink support

### Issues

* Funky stuff happens when using latitude slider
	* Is this our error or a SunCalc.js error?


## [Sun Azimuth Altitude OBJ Viewer]( http://ladybug-analysis-tools.github.io/ladybug-web/sun-azimuth-altitude-obj/ )

Latest update: 2016-03-06 / R1

### Features
* Built on [SunCalc]( https://github.com/mourner/suncalc )
* Creates a 3D Sun path
* Displays Sun times and position in radians and degree
* Set the date and time
* Loads and displays OBJ files - with shade and shadow
	* Includes five samples
* API that creates and accepts permalinks

### Things to Do / Road Map

* Rotate default buildings to correct orientation
* Fix azimuth/altitude error
* Allow for updates that don't reset parameters
* Faster ways for setting data and time


## [SunCalc Sandbox]( http://ladybug-analysis-tools.github.io/ladybug-web/suncalc-sandbox/ )

### Features

* Built on [SunCalc.js]( https://github.com/mourner/suncalc )
* Calculates and reports Sun times and position in radians and degrees
* Calculates and reports Moon illumination, times and positions in radians and degrees
* API that creates, updates and accepts permalinks
	* Accept date, time, latitude and longitude
* Buttons provide data for selected cities


### Latest update: 2016-03-14 / R7

* Code clean-up
* Display data in UTC plus in the time zone of the remote location
* Redesign permalinks
* Add buttons

<!--
### Permalinks

* [Barcelona Pavilion]( ./suncalc-sandbox/index.html#yr=2016#mo=1#da=1#hr=12#mn=0#la=41.3706#lo=2.1500 )
	* [SunCalc.net]( http://suncalc.net/#/41.3706,2.1500,12/2016.01.01/12:00/1 )
	* [SunCalc.org]( http://suncalc.org/#/41.3706,2.1500,12/2016.01.01/12:00/1 )
* [Robie House, Chicago]( ./suncalc-sandbox/index.html#yr=2016#mo=1#da=1#hr=12#mn=0#la=41.7898#lo=-87.5959 )
	* [SunCalc.net]( http://suncalc.net/#/41.7898,-87.5959,12/2016.01.01/12:00/1 )
	* [SunCalc.org]( http://suncalc.org/#/41.7898,-87.5959,12/2016.01.01/12:00/1 )
* [Schroder House, Utrecht]( ./suncalc-sandbox/index.html#yr=2016#mo=1#da=1#hr=12#mn=0#la=52.0853#lo=5.1472 )
	* [SunCalc.net]( http://suncalc.net/#/52.0853,5.1472,12/2016.01.01/12:00/1 )
	* [SunCalc.org]( http://suncalc.org/#/52.0853,5.1472,12/2016.01.01/12:00/1 )
* [Sydney Opera House]( ./suncalc-sandbox/index.html#yr=2016#mo=1#da=1#hr=12#mn=0#la=-33.8587#lo=151.2140 )
	* [SunCalc.net]( http://suncalc.net/#/-33.8587,151.2140,12/2016.01.01/12:00/1 )
	* [SunCalc.org]( http://suncalc.org/#/-33.8587,151.2140,12/2016.01.01/12:00/1 )
* [Villa Savoye, Poissy]( ./suncalc-sandbox/index.html#yr=2016#mo=1#da=1#hr=12#mn=0#la=48.9231#lo=2.02658 )
	* [SunCalc.net]( http://suncalc.net/#/48.9231,2.02658,12/2016.01.01/12:00/1 )
	* [SunCalc.org]( http://suncalc.org/#/48.9231,2.02658,12/2016.01.01/12:00/1 )
-->

### Issues

* More testing need to confirm times are correct


### Things to Do / Road Map

* Separate into engine and viewers  << 2016-03-08 separation process just starting with R5
* Select locations from a gazetteer of with lat/lon of over 2,000 places names
* Select lat/lon by clicking on a map or globe
* Click on each item of Sun times to update Sun position. Ditto Moon
* Highlight with color currently selected location


### Notes / Remarks

* SunCalc accepts dates both as ASCII and UNIX timestamps in milliseconds


## [Sun Azimuth Altitude]( http://ladybug-analysis-tools.github.io/ladybug-web/sun-azimuth-altitude/ )

Embedded description: _Set date and time. Set the location to any lat/lon. Adjust the view. View the Sun azimuth, altitude and shadows for that place and time. Permalinks created on the fly._

Latest update: 2016-03-06 / R3

### Features

* Set date and time
* Set latitude and longitude
* View Sun azimuth and altitude
* View shadow simulation
* API that creates and accepts permalinks

### Things to Do / Road Map

* Menu works on mobiles
* Select lat/lon by clicking on a map or globe
* Add gazetteer?
* Insert OBJ, JSON and other files into the scene
* Pick up 3D data from Google Street View - follow Callum Prentice


## Issues of Interest

https://github.com/ladybug-analysis-tools/ladybug-web/issues/1

## Links of Interest


[Sun Path in WebGL]( http://www.pycheung.com/weblog/?p=1394 ) 
* Shows how Analemma are created ~ [PY Cheung]( http://www.pycheung.com/weblog/ )
* No code or explanation

[Sunlight Hours Ladybug Dynamo]( http://hydrashare.github.io/hydra/viewer?owner=mostaphaRoudsari&fork=hydra_1&id=Sunlighthours_Ladybug_Dynamo&slide=0&scale=2.7215798676177987&offset=-765.8096117029108,-203.1389988323118 )
* Here it is in Python. Can we do it in JavaScript?
* [Source]( https://github.com/ladybug-analysis-tools/ladybug-core/blob/master/ladybug/sunpath.py#L97-L138 )


[SunCalc]( https://github.com/mourner/suncalc ) ~ Thank you [Vladimir Agafonkin]( http://agafonkin.com/en/ )!

[Astronomy Answers ~ Position of the Sun]( http://aa.quae.nl/en/reken/zonpositie.html )

[SunCalc.net]( http://suncalc.net/ ) ~ Vladimir Agafonkin!
* You must use the time of the local computer location. 
	* In order to see sunrise in Europe from a computer in San Francisco, you must set time as, say, 23:50
 

[SunCalc.org]( http://www.suncalc.org/ ) ~ [Torsten Hoffman]( http://www.torsten-hoffmann.de/ )  
[MoonCalc.org]( http://www.mooncalc.org ) ~ [Torsten Hoffman]( http://www.torsten-hoffmann.de/ )  
* These apps also use the time at you current location
	* But also displays local time at the location being viewed

[NOAA Solar Calculator]( http://www.esrl.noaa.gov/gmd/grad/solcalc/index.html )
* [Main JavaScript routine]( http://www.esrl.noaa.gov/gmd/grad/solcalc/main.js )
* Main page fairly easy to update
* Calls them 'azimuth' and 'elevation'
* Does not give negative elevations


[Sun Earth Tools]( http://www.sunearthtools.com/dp/tools/pos_sun.php ) ~ no API ~ UK app - no authors listed

[Sun  Path 3]( http://andrewmarsh.com/apps/releases/sunpath3d.html ) ~ no API ~ [Dr Andrew Marsh]( http://andrewmarsh.com/ )

[Solar Path]( http://bl.ocks.org/mbostock/7784f4b2c7838b893e9b#solar-calculator.js ) ~ Mike Bostock

[NOAA Solar Calculator]( http://www.esrl.noaa.gov/gmd/grad/solcalc/ ) ~ Find Sunrise, Sunset, Solar Noon and Solar Position for Any Place on Earth
* http://www.esrl.noaa.gov/gmd/grad/solcalc/emaps.js
* Previous version: http://www.esrl.noaa.gov/gmd/grad/solcalc/azel.html

[Sun Position Calculator]( http://www.pveducation.org/pvcdrom/properties-of-sunlight/sun-position-calculator )


http://www.metafilter.com/130877/SunCalc-a-solar-azimuth-calculator

http://www.analemma.com/Pages/indexPage.html
* Old and has issues




***

<center title="dingbat" >
# <a href=javascript:window.scrollTo(0,0); > ❦ </a>
</center>
