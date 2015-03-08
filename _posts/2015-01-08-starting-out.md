---
layout: page
categories: electronics_tutorial beginner
title: "Starting Out: Where To Begin"
permalink: /asdet/starting-out
---

This is part of my [slightly different electronics tutorial][asdet] series.

So, you've read about these newfangled electronic gizmos that are poised to enter rampancy and take over the world, and you'd like to try your hand at building some.  So, you head over to your local "electronics" shop, and ask the friendly salesperson wandering around the aisles where the Arduino boards are kept. They give you a strange little laugh and an odd look, parroting _"Ahdweenohs? I don't think we stock those here"_ whilst you stand there, more than a little disappointed.  Unfazed, you turn to the Internet and stumble apon the millions of kits out there.  Which ones are better? What should you be looking for?

To be honest, it's much more fun putting together a set of equipment that you know you will use, rather than cluttering up your workspace with all sorts of parts that will never be used and just take up space.  I wouldn't bother with any of the shiny _"XYZ-compatible"_ systems with esoteric connectors or cute-looking cases -- more often than not you'll find yourself limited by what they can do rather than the other way round, and many of them are locked into a specific form-factor with expensive add-on boards for basic sensors.  Sure, they make it easy to start, but once you're ready to go beyond the basics, they can make it a lot harder than it should be.

With these issues in mind,  I've written up this list to help you know what to look for in a prepackaged "beginner's" kit, if not source directly.  I assume you have access to a computer you can install programs on, but there's a whole bunch of other parts you'll need as well. The bare minimum you'll need to begin with is:

### Core digital electronics board:

- **[Arduino UNO](http://arduino.cc/en/Main/ArduinoBoardUno)**, or a clone.  It costs around $15-30 and it's __SHINY!__ But it's only 8-bit... most new computers have 64 of those!  Why should you start with 8?  One reason is that it's a lot easier to wrap your head around how the comparatively tiny Arduino works than that of a modern computer, and it's suited to different tasks too.  You can do away with all the fancy Arduino IDE fluff later and this board is still a pretty useful platform for the ATMEGA328 chip.

    Due to its popularity there are plenty of copies out there from different manufacturers, adding all sorts of features.  Stick to something simple for now, unless you know you'll need a specific feature later down the track.  With this in mind, some good alternatives to an Arduino-made board are the [Freetronics Eleven](http://www.freetronics.com.au/products/eleven) in Australia with its extra prototyping area, or the [Sparkfun Redboard](https://www.sparkfun.com/products/12757) in the U.S. with its surface-mounted everything, resulting in a nice flat back surface.  Both come with Micro-USB ports for programming instead of the original Arduino's USB-A port, which means they won't short out some of the expansion boards ("shields") out there like the original Arduino occasionally does.

    If you're looking for really inexpensive because you don't have much money -- or just can't justify the 50-100x larger price tag to support the original designers -- the cheapest clone I have ever seen is the DCcduino which can be found for under $3 [if you shop around][aliexpress], but [installing the drivers][drivers] to talk to it can be difficult if you [don't know where to look][dccdrivers].

- **USB cable.** I have a box of all sorts of different varieties, but you really only need a USB A (if you're using a real UNO it comes with one) or a Micro-USB cable (if using an Eleven, Redboard, or many other clones).

### Tools:

- **Breadboard.**  No, not that kind! _canned laughter_ Still, a wooden breadboard is great for cutting up components and wires at a later stage in this tutorial.

    Don't worry too much if you don't know how a solderless prototyping board works yet. A good mid- or full-size one will be fine.  Try and get the modern(?) ones if you can help it (they are usually white whilst the older types are cream/beige, and snap rather than slide together), since they're more compact than the old kind (which have quite a wide ridge), and many handy breadboard-based circuits (such as mini power supplies) are built to fit straight onto them.

- **Jumper wires.**  Somewhat odd name, but it makes sense if you come from an electronics background.  These are basically pieces of wire to plug in and connect things together.  You're going to need different types and lengths; I recommend getting some high quality "DuPont" connector wires (Male-Female and Male-Male are really useful) as well as plain old insulated solid-core wire with bare ends.

    Don't try and make your own out of stranded wire unless you're prepared to tin the ends with solder. Even then it's a nightmare to use for prototyping, and generally not worth the cheaper price -- just go for solid core and save yourself precious time.

- **Digital Multimeter.**  Any kind will do a good enough job for learning, so just look out for one within your price range.  Try to grab one that's capable of measuring resistance and capacitance -- these are really useful when you are trying to find the right component, and you haven't yet memorised the resistor colour charts or joule conversions!

- **Precision screwdriver set** for all those tiny screws everything uses.  The small flathead screwdrivers also double as a light duty pry-bar in a pinch, which is useful for moving a pesky stuck jumper wire in a crowded circuit.

- **Needle-nose pliers** for straightening out wires, bending component leads, placing small parts and other miscellaneous tasks that require good grip and dexterity. The thinner at the tip, the better.

- **Parts box** to store all of your electronics in.  Anything with lots of (smallish) compartments is fine.

- **Resistor colour band translator** of some kind.  [I recommend Adafruit's excellent one that you can make yourself!](http://www.adafruit.com/blog/?p=30272)

### Basic components (the bread-and-butter of circuits):

- **Resistors** -- used to reduce or restrict the flow of electricity around the circuit.  220Ω, 330Ω and 10KΩ are the most common values in circuits, but you'll need a few other values for projects beyond the basic level.  All standard values between 0Ω (AKA a piece of wire) and 1MΩ (basically considered an open circuit) are good to have.  If you're unsure where to start, try something like [Sparkfun's resistor kit](https://www.sparkfun.com/products/10969).

- **Power supply** of some kind -- this can be a 9V battery with some wires to stick into your breadboard power rails, a 4xAA box, a USB cable to your Arduino or even a huge overpowered desktop bench supply; it doesn't really matter as long as it can produce 5V.

### Input:

- **Push buttons,** any size will work well enough, but the smaller the better for price and fitting in a crowded circuit. As well as using them as a control method for circuits, you can use these as touch or bump sensors, as well as momentary switches.

- **Potentiometer** -- fancy resistors that have a dial to go from 0Ω up to a set value.  10KΩ and 1MΩ are good values to have.

- **LSR or photocell** -- light sensitive resistors make for a good sensor for all sorts of projects involving light!

- **Analog temperature sensor** -- the TMP36 is a common one, and good for starting out. Analog temperature sensors are generally easier to get to grips with though, at the cost of lower accuracy when compared to digital ones.

- **IR phototransistor** -- a fancy way of saying "part that detects infrared light, or heat", useful for if you want to control anything with a TV remote, or pick up infrared signals.

### Output:

- **LEDs** of all shapes and sizes, as many as you like!  You can never have enough blinking lights in a circuit.

- **Infrared LED** -- shines light in the infrared range that can be picked up by an IR phototransistor (like on a TV or another circuit).

- **Speaker** -- some clones might have one built in, but usually you need to buy this separately.  _Don't confuse this with a buzzer!_ They are two separate things.  A speaker can do every tone under the sun; a buzzer has only one tone and isn't as fun to use (even though they're generally cheaper!)

- **LCD display** to have a text interface for what your microcontroller is doing.

### Not necessary to start out with, but nice to have

I'm not sure how useful these items are for a true beginner -- those that I know like to have instant results without much effort -- but I like playing around with them so they're here for completeness:

- **Capacitors** -- sort of like mini batteries that hold a charge for a very short time.  You don't need a huge range of these.  Having an assortment of values in the 10-100uF range is useful, stick to ceramic and electrolytic (polarised) kinds for now -- the other kinds tend to be for more esoteric applications than learning electronics.
- **Transistors** -- used to amplify quiet signals or act as a simple electronic switch. The most well-known numbers are 2N3904 and 2N3906 for a good solid NPN and PNP transistor respectively.
- **Motors** -- a simple DC motor is a good place to start, but also get a stepper motor to get more accuracy in your movement.  For real control and accuracy in movement, try a servo motor -- I'd suggest starting with a standard servo (180 degrees of rotation) since continuous rotation servos are a little tricky to understand until you learn where their controls are coming from in the 180 degree world.
- **Diodes** -- the "one-way valves" of electronics.  Buy a couple of Zener diodes (part numbers 1N4678 to 1N4717) as well as small power diodes (any sporting the mark "1N4001" or "1N4000" will be fine).
- **MLX90614 contactless thermopile.** This is a contactless IR sensor that has really good accuracy for detecting infrared temperatures
- **Ultrasonic distance sensor** -- the most common "beginner-friendly" sensor is the HC-SR04, which isn't terribly accurate but _good enough_ for most purposes.
- **Ethernet shield** to connect your newly found microcontroller to the WWW. IoT ALL OF THE THINGS!
- **7-segment display** if you feel like practicing multiplexing and timing!
- **555 Timer IC (Integrated Circuit)** -- you'd be surprised just how much can be done with this one little timer chip!  Definitely consider including one of these, if not a 556 IC (two 555s in one chip).
- **L293N motor driver IC** -- this will drive DC and stepper motors for you, so you don't have to worry about the high amount of current that motors need blowing up your other electronics.
- **74HC595 shift register IC** -- the easy way to get more digital pins onto your Arduino.  These control 8 digital outputs at the cost of 2 pins on your Arduino board, and you can easily build a chain of these to control even more pins if you want to.  I highly recommend playing with one of these if only to wrap your head around basic multiplexing and the I2C communication protocol.
- **SPDT relay** -- Single Pole Dual Throw (SPDT) relays are a quick way to isolate and control an electric circuit at a higher or lower voltage from your electronics boards.  Think of them like an electrically-controlled switch to turn on/off other circuits.

### TL;DR: Just give me a parts checklist!

Okay, okay...

- Arduino UNO or equivalent board with an ATMEGA328 at its heart
- USB cable to connect it up to your computer
- Solderless Breadboard
- Jumper wires
- Digital Multimeter
- Precision Screwdrivers
- Needlenose pliers
- Parts Box
- A bunch of resistors (330Ω and 10KΩ are common, get a range of them if you're serious about/like resistance)
- A bunch of capacitors (a few in the 10-100uF range is fine)
- A couple of transistors (2N3904 and 2N3906)
- Two or three diodes (part no. 1N4678-1N4717, two or three of 1N4001/1N4000)
- 5V Power Supply for your breadboard/ Arduino
- Buttons (small ones are good)
- Potentiometers (10KΩ and 1MΩ)
- LSR/Photocell
- Analog temperature sensor (TMP36)
- IR phototransmitter
- IR LED
- Visible light LEDs
- Motors (DC, stepper, servo -- one of each kind or more)
- Speaker

# Next Time

[Where do I Buy Parts?][next]

[asdet]: /asdet
[iteadlite]: http://imall.iteadstudio.com/iteaduino-lite.html
[drivers]: http://www.jasinski.us/cheap-arduino-clone-dccele-dccduino-uno/
[dccdrivers]: http://javacolors.blogspot.fi/2014/08/dccduino-usb-drivers-ch340-ch341-chipset.html
[aliexpress]: http://www.aliexpress.com/wholesale?catId=0&initiative_id=SB_20150201203519&SearchText=arduino+uno
[next]: {% post_url 2015-02-02-where-to-buy %}
