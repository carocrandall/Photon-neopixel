# Photon-neopixel

Particle project

Goal – to have a matrix of buttons on a website remotely control a matrix of LED’s operated by a Particle Photon. 

a) How good is the documentation?
	The documentation by the Particle team is fairly impressive.  And overall complete.  They have a lot of straightforward examples and an online community similar to the Arduino platform.  However, they are a newer product so there is less documentation. 

b) Who’s tried this before?
	Not clear  - people have definitely tried attaching neopixels to the Particle photon.  There is documentation about the ring of neopixels and I believe the library is accessible on the Particle platform which is good. 
	There is a decent amount of people who have had problems – but it looks like the main problem there is that they needed a level shifter or a shield.  The photon supplies 3.3v and the neopixels need 5v. 

c) What have the outcomes been?
d) What are some examples?
	There is one interesting example I have come across of someone using this to make a whole “torch” of neopixels and that person has shared their process.  http://happyinmotion.com/?p=1247

There is another tutorial using “octoblu” but I am not sure what that is. 
https://www.hackster.io/virgilvox/web-enabled-neopixels-using-particle-octoblu-b4e8fa

http://core-electronics.com.au/tutorials/using-neopixels-with-particle.html


e) How complicated do those examples look?
	Unclear – I think it could be a problem that particle photon doesnt play nicely with CCA’s network. 
f) Does it require exotic libraries, languages, hardware, or other items?
	I don’t think so, other than the standard neopixel library from adafruit.  From Particles site: “You can include a library in an application by opening the library drawer, finding a library that will work for your project, and clicking the "include in app" button. This will add an #includestatement to your code that will expose all the capabilities of the library to your code.

g) What parts do I need to acquire?

Materials:
-	Particle Photon
-	USB micro cable
-	Stranded wire
-	8x8 Neopixel matrix
Either a level shifter http://www.digikey.com/product-detail/en/SN74HCT125N/296-8386-5-ND/376860
https://www.adafruit.com/product/1787 
OR a Photon shield https://store.particle.io/collections/shields-and-kits  
-	
-	Capacitor
-	480 ohm resistor
-	5v power supply

2) Once we determined that it seems feasible to proceed, we would want to find
a reasonable small study (example) to convince ourselves that we really can do
this. If this were Arduino we would do the ?blink? example. We are not
necessarily trying to do something useful, but to verify that we can make
anything work at all.
It took me almost three hours to get an unreliable blink happening on the CCA network and I was super disheartened by it.  I was so disappointed.  But once I was at  home on my own wifi it took less than 5 minutes. 
a) Hopefully, we would find a simple existing, well-documented example (ideally
a tutorial or similar)
b) If we couldn?t find an existing tutorial, we would have to design our own
example to demonstrate the correct usage of the tool/library/device/concept.
3) Next, we would look for a slightly more complicated example, though still
mostly trivial; this time relevant to whatever it is we want to be doing with
this tool. Again, ideally we find something already written by someone else,
but if necessary we?d design our own.
I found a tutorial that turns an LED on and off from a web page using particle that is along the lines of what I would want to do, and I got that up and running which was awesome. 

Notes:

1.	Understand the Particle Photon.  There is a lot of great documentation.  It is basically an wifi-enabled Arduino controlled via an api. 
2.	Particle has an integrated development environment or IDE called Particle Build – you use a web browser to develop apps.  
3.	The code used in this IDE is arduino format, which is great.  I have used that before but I am not an expert. 
4.	I am pretty certain that Adafruit neopixels require a library – and Particle has some documentation on that, but they could use more.  This could be a problem. 
“You can include a library in an application by opening the library drawer, finding a library that will work for your project, and clicking the "include in app" button. This will add an #includestatement to your code that will expose all the capabilities of the library to your code.
5.	This is firmware
6.	Found some examples – got some sample code running blinking an LED from an html page. 
7.	Looked at the online forums to get a sense of the problems – people reported some weird behavior
8.	One thing I have noticed as a heads up – the neopixels need 5v the photon supplies 3.3v .. recommend a level shifter. 
A possible tutorial but I am not sure what this octoblu thing is 

uses a rest api – what is that?

https://github.com/technobly/SparkCore-NeoPixel 

https://learn.adafruit.com/adafruit-neopixel-uberguide/basic-connections 



