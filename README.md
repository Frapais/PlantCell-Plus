# PlantCell-Plus

This is the repository of my **PlantCell Plus** project, a complete plant monitoring system, consisting of a Capacitive Soil Moisture Sensor, an Ambient Light sensor, and an Air Temperature & Humidity sensor.
By directly soldering a NanoCell board, you can make a battery powered plant monitoring sensor for Home Assistant.

|<img src="https://github.com/Frapais/PlantCell-Plus/blob/main/Photos/2024-05-15T21_10_45.301Z-2024-05-15%20033.jpg" alt="Photo1" width="600"/>|<img src="https://github.com/Frapais/PlantCell-Plus/blob/main/Drawings/Plant%20monitor%20pinout.png" alt="Pinout" width="200"/>|
|-|-|




## Description
### Hardware
The soil moisture is measured by measuring the varying capacitance of the sensor's surface. If everything else stays constant, the capacitance will change with the change of the water content in the soil.
The sensor outputs an varying voltage corresponding to the change in capacitance, which we can measure via an analog input of any microcontroller.

#### Main Features
* Corrosion-resistant soil moisture sensor
* I2C Ambient light sensor
* I2C Air temperature & humidity sensor
* GPIO-controlled power supply for low power consumption
* LiPo battery connector

### Tests
To test this sensor, a NanoCell-C3 board was soldered to the corresponding pins, and the raw values of the sensor were continously uploaded to the local Home Assistant server.
The analog input was read with 11dB attennuation, and the maximum values were **1.8V** with a completely dry sensor, and **0.89V** when the sensor was submerged in a glass of water.
These valuse can be mapped into a percentage of **0%** and **100%** soil moisture accordingly. However, it is recommended to repeat this calibration process when the sensor is placed inside the soil in its final position.

### Initial Home Assistant setup
#### Requirements:
* Access to Home Assistant Dashboard
* Installed ESPHome plugin

#### Setup process:



## Availability
You can get the assembled boards from my [Official Website](https://frapaislab.com/smart-soil-moisture-sensor), and from [Tindie](https://www.tindie.com/products/frapais/plantcell-plus/).

<a href="https://www.tindie.com/stores/frapais/?ref=offsite_badges&utm_source=sellers_Frapais&utm_medium=badges&utm_campaign=badge_large"><img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-larges.png" alt="I sell on Tindie" width="200" height="104" allign="left"></a>



## Support
If you find this project useful, please consider supporting me on any of the following platforms:
* PayPal:
  * <a href="https://www.paypal.com/paypalme/kostasparaskevas">
    <img src="https://img.shields.io/badge/$-donate-ff69b4.svg?maxAge=2592000&style=flat">
* Buy Me a Coffe:
  * <a href="https://www.buymeacoffee.com/frapais" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px     3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
* Instagram:
  * [@frapais.lab](https://www.instagram.com/sprig_labs/)
