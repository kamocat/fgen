# fgen
A simple amplifier for a phone-based function generator

You'll need to install an app on your phone to actually generate the signal.
I recommend this one: https://play.google.com/store/apps/details?id=com.keuwl.functiongenerator

## Update:
It turns out the function generator does a pretty poor job of generating square waves above 1kHz, and the triangle waves are marginably passable. This could be a problem with the phone or the slew rate of the op-amp. I didn't have any capacitors larger than 100uF, so it can really only put out 50mA at full voltage. To top it off, the the function generator output depends on the phone's volume settings, and the offset feature doesn't work (probably due to a decoupling capacitor in the phone). Maybe I should switch to an MQTT-controlled ESP32.
