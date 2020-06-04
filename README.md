# lgtm

This is a guide for creating your own physical LGTM stamp that actually approves code. The stamp contains a microcontroller, battery, and inductive charging coil. It is connected to a computer via Bluetooth. When the onboard accelerometer records a "stamp", a keypress is sent to the computer. A Chrome extenion listens for this specific keypress and if the browser is currently viewing a Github pull request, the PR is approved. 

## Demo

[![LGTM stamp demo](http://img.youtube.com/vi/ngm4KjQLanQ/0.jpg)](http://www.youtube.com/watch?v=ngm4KjQLanQ)

## Hardware

You will need the following hardware:
* An [Adafruit Feather Sense](https://www.adafruit.com/product/4516) microcontroller
* A [500mAh lithium ion polymer battery](https://www.adafruit.com/product/1578) to power the microcontroller
* A [universal Qi wireless receiver module](https://www.adafruit.com/product/1901) to charge the battery
* A [3d printed shelf](shelf/shelf.stl) designed specifically for this project to properly position the Qi receiver module
* A Qi charging pad. Any of them will do, but I like [this one](https://www.amazon.com/gp/product/B00F1SHFJA/) because it's the same physical size as the stamp.
* A 2"x5" LGTM rubber stamp from [Rubber Stamp Champ](https://www.rubberstampchamp.com). You will need to order it twice because they **always** mess up the first order. Ask them to ship it disassembled.
* [2" self-adhesive industrial strength velcro](https://www.amazon.com/Strenco-Adhesive-Black-Hook-Loop/dp/B00H3R9S1K/) for afixing the rubber LGTM piece to the wood block of the stamp
* Six #2 x 1/4" brass screws because brass is class

This project also requires a bunch of tools. See the Construction section for details.

## Software

There are two pieces of software that you'll want to customize for your needs before using.

### Arduino

### Chrome extension

## Construction

To begin, you'll need to hollow out the center of the stamp's wood block. The cutout should be centered and measure 4" long, 2" wide, and about 1/2" deep. To do this, I clamp the wood block to a workbench, use some painter's tape to mark 1/2" on a 1/4" drill bit, and drill tons of holes. I then remove the remaining wood with a hammer and wood chisels. A router would probably be amazing for this, but I just don't have one. Glue the handle in place.

Stick the coarse "hook" side of the velcro onto the back of the LGTM rubber piece. Trim the bottom of the stamp's wood block with the soft "loop" side of the velcro. 

Solder a couple wires from the Qi receiver to the `USB` and `Gnd` pins on the Feather. 

Soft-fit everything first so you can see where it goes. Then use four screws (or however many you want) to secure the Feather to the stamp. Connect the battery to the Feather place it beside the Feather. Place the shelf above the Feather and battery, center it to the cutout and secure with two screws. Affix the battery to the stamp with some double-sided tape. Finally, glue the Qi receiver to the top of the shelf. 
