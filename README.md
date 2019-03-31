# connecting teensy 3.6 mcu to cs42448
Eagle schematic for [cs42448](https://statics.cirrus.com/pubs/proDatasheet/CS42448_F5.pdf) codec + teensy 3.6 (with passive filters)

Based on circuit description from Paul Stoffregen [here](https://forum.pjrc.com/threads/41371-Quad-channel-output-on-Teensy-3-6?p=138969&viewfull=1#post138969)


# circuits

## codec
* 4 stereo inputs 
  * non-differential inputs
  * passive input filters
* 4 stereo outputs (using single-ended outputs)
  * non-differential outputs
  * passive output filters
![cs42448](/images/cs42448.png)

## teensy 3.6
![cs42448](/images/teensy.png)

## audio input module (ST_IN)
![cs42448](/images/input.png)

## audio output module (ST_OUT)
![cs42448](/images/output.png)
