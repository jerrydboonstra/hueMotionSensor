## Hue motion sensor (for SmartThings integration, no Hue bridge)

**Motion:**
Very snappy, works better than original smartthings motion sensor (even if the DTH runs in the cloud) having no delay or sleep time for reporting the motion events.

Also you can configure the following:
* Motion sensitivity (Low, Medium, High). Default is High

**Temperature:**
It's accurate and reported in time. You can also correct the readings by configuring an offset.

**Illuminance:**
It's accurate and reported in time. You can also correct the readings by configuring an offset.

**Battery:**
Used the same logic as the smartthings motion sensor. Seems accurate.

# Forked from bogdanalexe90's project to handle the hue outdoor motion sensor

# Installation
* Create a new DTH from code 
  * Integrate directly with the Github repo
  * Or, create a new custom DTH from code
    * Login to [https://graph.api.smartthings.com/ide/devices](https://graph.api.smartthings.com/ide/devices) and create a new device handler, using the Code method.
    * Paste one of the following files contents, depending on your model
      * Use [hue-motion-sensor.groovy](devicetypes/bogdanalexe90/hue-motion-sensor.src/hue-motion-sensor.groovy) for the original indoor Hue Motion Sensor
      * Use [hue-outdoor-motion-sensor.groovy](devicetypes/bogdanalexe90/hue-motion-sensor.src/hue-outdoor-motion-sensor.groovy) for the original indoor Hue Motion Sensor
    * Save and publish the DTH
* Reset your device by pressing the setup button until device led starts to change color (~15 sec).
* Open your Smartthings app and search for a new device
  * When found, you can rename the device before adding it
* You can now create Automations triggered by the device
