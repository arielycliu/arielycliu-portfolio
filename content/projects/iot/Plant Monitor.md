---
title: IoT Plant Monitor
draft: false
tags:
 - Arduino
 - ESP
 - Twitter
 - IoT
---
##### [Check out the article here](https://arielycliu.medium.com/get-alerted-when-your-plants-dying-d085d0bdedf5)

##### [Check out the Github here](https://github.com/arielycliu/MicrocontrollerProjects/tree/master/ESP/Smart%20Plant%20Project)


## 🌵Inspiration
My succulent died :(

Actually all of my succulents died, I had a whole pot of them and *none* of them survived 💀

I think that could almost be considered impressive.

## 🔍What it does
Notifying a plant’s health with an ESP moisture monitoring system by tweeting the moisture level every five minutes 💦
The plan here is when the soil is too dry, I’ll receive a **notification** on my phone to water it. The ESP will consistently check the moisture, display real-time moisture data on my phone, and **tweet** it using my ~twitter~ (I mean X) account.

With both notifications and tweets there's no way the plant still dies right?

![Flow diagram of iot setup](https://miro.medium.com/v2/resize:fit:720/format:webp/1*6ssnfdV3tSzf6yhTMSHWew.png)

![Image of my build](https://miro.medium.com/v2/resize:fit:720/format:webp/1*Y0BS4PfH1UjNNGgDArdSCw.jpeg)


---


## 🔨How I built it

I used an ESP as the microcontroller for this project, and brought a nice new moisture sensor called the Flying Fish Soil Moisture sensor. The probes are able to measure the amount of water in the soil. The amount of **voltage** that the sensor returns to the ESP depends on the moisture level. Between the probes, an electric current runs through the soil. The more water content there is in the soil, the more electricity can be conducted. On the flip side, when the soil is dry, there is more **resistance** and less electricity is conducted. 
I just hooked it up to my ESP like so (ignore the fact that the image is clearly an Arduino, it's the same pins).
![Hardware wiring diagram](https://miro.medium.com/v2/resize:fit:720/format:webp/1*AEWjuFN1LO-hRbr3rz1e1w.png)
Here's another diagram with the right kind of microcontroller but the wires are kind of hard to see and I couldn't drag them like in Tinkercad (created in circuito.io)
![Diagram two with an esp this time](https://miro.medium.com/v2/resize:fit:720/format:webp/1*o8cgccATDaz2acwyAL9PqQ.png)

For this project, I chose to use the [Blynk IoT platform](https://blynk.io/) to record the data, **tweet**, and send **notifications**. I connected my ESP to the Internet to get the current time using the Network Time Protocol (the standard IP that computer synchronize to). Then I just set up Blynk to help tweet the time and moisture data from my ESP. I also downloaded the Blynk App so that I could get notifications reminding me to water the plant. 🚿

(The downside of this project is that my twitter account now looks like a bot account.)
![My twitter account](https://miro.medium.com/v2/resize:fit:720/format:webp/1*TFkJR3YQ6AqsY5GICBhMRQ.png)

[Check out the article to learn more](https://arielycliu.medium.com/get-alerted-when-your-plants-dying-d085d0bdedf5)
