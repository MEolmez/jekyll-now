---
layout: post
title:  "Arduino low power ds18b20 temperature probe with display"
date:   2018-01-20 16:16:01 -0600
categories: arduino 
---

I wanted to make a waterproof temperature probe with a low current consumption. 

First part is the ds18b20 with a waterproof casing.

Second part is 4 digit display with TM1637 chip. I find these kind of displays very useful , even though they only have 4 digits sometimes thats all you need.

I wanted this project to use very little current , so i used an arduino pro mini 3.3v. 

For further reducing the current consumption i set the displays brightness to lowest and used a sleep mode so arduino only wakes up at 2 second intervals , takes the measurement , updates the display , and sleeps again.
This way project uses 6ma. Its possible to further reduce this values by using the internal pull up resistor for ds18b20 and removing the onboard power led from arduino.



Code is <a href="https://github.com/MEolmez/arduino-ds18b20-temperature-probe-with-display">HERE</a>


![usefulimage]({{https://meolmez.github.io}}/assets/tempProbe.jpg)




