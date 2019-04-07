# connecting teensy 3.6 mcu to cs42448
Eagle schematic for [cs42448](https://statics.cirrus.com/pubs/proDatasheet/CS42448_F5.pdf) codec + [teensy 3.6](https://www.pjrc.com/store/teensy36.html) (with passive filters)

Based on discussion from [pjrc forum](https://forum.pjrc.com/threads/41371-Quad-channel-output-on-Teensy-3-6) about circuit  described [here](https://forum.pjrc.com/threads/41371-Quad-channel-output-on-Teensy-3-6?p=138969&viewfull=1#post138969)
* reference pcb available from [oshpark project](https://oshpark.com/shared_projects/2Yj6rFaW)

# work-in-progress
* This circuit has not been produced, verified or reviewed. 
* Please feel free to suggest corrections, improvements, raise issues, etc.

# to-do
* verify if decoupling caps for VA should be before or after the ferrite bead.
* verify if CAT811T reset is wired correctly. 
* verify if PIN1 / CS is setup correctly with two resistors and solderable pad options. 

# circuits

## codec
* 3 stereo inputs 
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
