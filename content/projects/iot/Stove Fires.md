---
title: Stove Fires
draft: false
tags:
  - Arduino
  - ESP
  - Twitter
  - IoT
---
##### [Check out the article here](https://arielycliu.medium.com/preventing-fire-with-iot-a-simple-solution-c42853dde7fe)

##### [Check out the Github here](https://github.com/arielycliu/MicrocontrollerProjects/tree/master/ESP/Temp%20Monitor%20Project)


## 🍳Inspiration
My grandma often forgets to turn off the stove, leaving it lit throughout the night. Other than being a huge waste of fuel, it can also be quite dangerous if a fire did catch. And no, I do not want my house evenly roasted.

## 🔍What it does
I connected a TMP temperature sensor to my ESP32, a microcontroller similar to Arduino but with the capability of connecting to wifi. Then using the Arduino IDE I programmed my ESP to receive the data, connect to my home’s wifi network, and send the data to the ThingSpeak API. From there ThingSpeak does the rest, storing and graphing the data in real-time.

Here's what the plan looks like:

![Flow diagram of iot setup](https://miro.medium.com/v2/resize:fit:720/format:webp/1*AGIZb2oTMdqPq0u9TPo_8g.png)

![Image of my build](https://miro.medium.com/v2/resize:fit:720/format:webp/1*mPkwsnUoYPW8ThWNTWS-CQ.png)


---


## 🔨How I built it

I used an ESP as the microcontroller for this project, it's a chip microcontroller that was designed for low power consumption at a low cost. I used the ESP32 Dev Module, partially because it was designed with smart wearable applications in mind, and mostly because it's something I already got for free at a previous tech camp. 

![Hardware wiring diagram](https://miro.medium.com/v2/resize:fit:720/format:webp/1*2jp_K9MA86esNPkYoxo0HA.png)

The tricky sending data part comes down to ThingSpeak. 
ThingSpeak is a good analytics platform, created for IoT applications. Using their server, API, and channels I could send data from my ESP to ThingSpeak and monitor it in realtime. I send the temperature data to the ThingSpeak API to get a nice graph monitoring my kitchen temperature.

![Temperature graph](https://miro.medium.com/v2/resize:fit:640/format:webp/1*5ELq4yuGllrM9Y459VpFHA.png)