
Purpose of Test: This tests aims to verify that the RPi sensor submerged in transformer fluid is able to detect tones underwater

Date: 2024/01/02
## Bill Of Materials

- [x] USB to Ethernet adapter
- [x] RPi Sensor
- [x] DC power supply for RPI
- [x] Laptop
- [x] Laptop Charger
- [x] Double Adapter
- [x] Phone charger adapter (in case dc fails)
- [x] plastic bag for phone to be submerged in - make sure bag is big enough for phone
- [x] Phone with tone generator
 ----
## Preparatory Procedure

- [x] Verify one can communicate with RPi on IP `192.168.1.101`
- [ ] Record commit SHA of RPi sensor
- [x] Verify one static IP address is `192.168.1.103
- [ ] Verify RPi sensor is configured to:
	- [x] Transmit at `44100 Hz`
	- [x] Connect on port `10000`
	- [x] Transmit to IP `192.168.1.103`
- [x] Verify proc server is on PC
- [ ] Record Proc server version
- [x] Very Proc server is configured to:
	- [x] Listen for connections on port `10000`
	- [x] WAV pipeline is set to `True`
	- [x] WAV recording is set to `True`
- [x] Take notes on testing environment
	- [x] What are you testing in  - Pool/Sea
	- [x] If pool 
		- [x] what are the dimensions
		- [x] Is the water heated
		- [x] Salt of chlorine 

----
## Test Environment

- Pool is 7x3m
- Water cool to the touch - not freezing
- chlorine pool
- Device places on top step - just submerged += 8cm underwater

----
## Test Results

#### Audio_fs_44100_Chans_4_1704204938_AirTest
- Air Test - knocking on the device, some clicks as well.
- Demoed to hosts father
#### Audio_fs_44100_Chans_4_1704205854_Ambient.wav
- Ambient pool environment
#### 255 Hz
- Audio_fs_44100_Chans_4_1704206028_255
- Audio_fs_44100_Chans_4_1704206059_255
- phone in bag
- could hear the sound
- not fully submerged
#### 50 Hz
- Unsure if 50 Hz was playing or not - it was not

----
## Sources of Issue

- Can hear TX out of water - large matching loss from phone
- Standing wave formation in pool - no idea what that does to the system
- Device on top step - step could act as a physical filter?

----
## Notable Results

- Mic did not transmit 50 Hz data
- Ambient mic data looks like this - channel 1 zoomed in:
![[SpectrogramAmbientEnv.png]]  
- Mic data with 2000 Hz - channel 1 zoomed in
![[Spectrogram2000Hz.png]]
----
## Conclusion

- Look Like it the device is able to detect tones under water
- The mics are very noisy...



