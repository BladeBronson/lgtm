# lgtm

This is a guide for creating your own physical LGTM stamp that actually approves code. The stamp contains a microcontroller, battery, and inductive charging coil. It is connected to a computer via Bluetooth. When the onboard accelerometer records a "stamp", a keypress is sent to the computer. A Chrome extenion listens for this specific keypress and if the browser is currently viewing a Github pull request, the PR is approved. 

## Demo

[![LGTM stamp demo](http://img.youtube.com/vi/ngm4KjQLanQ/0.jpg)](http://www.youtube.com/watch?v=ngm4KjQLanQ)

## Hardware

You will need the following hardware:
* An [Adafruit Feather Sense](https://www.adafruit.com/product/4516) microcontroller
* A [500mAh lithium ion polymer battery](https://www.adafruit.com/product/1578) to power the microcontroller
* A [universal Qi wireless receiver module](https://www.adafruit.com/product/1901) to charge the battery
* A Qi charging pad. Any of them will do, but I like [this one](https://www.amazon.com/gp/product/B00F1SHFJA/) because it's the same physical size as the stamp.
* A 2"x5" LGTM rubber stamp from [Rubber Stamp Champ](https://www.rubberstampchamp.com). You will need to order it twice because they **always** mess up the first order. Ask them to ship it disassembled.
* [2" self-adhesive industrial strength velcro](https://www.amazon.com/Strenco-Adhesive-Black-Hook-Loop/dp/B00H3R9S1K/) for afixing the rubber LGTM piece to the wood block of the stamp
* Six #2 x 1/4" brass screws because brass is class

## Software

## Construction
