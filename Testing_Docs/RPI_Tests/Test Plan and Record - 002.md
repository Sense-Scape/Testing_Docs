
Purpose of Test: This test aims to check if I can get constant phase between two channels

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
- Device places on top step - just submerged += 20cm underwater

----
## Test Results

- [Data Location](https://mega.nz/file/9q1w3JSZ#VH06QL7HJrUOSN9voN9jmmloAQyCWSXpJxuRHwPFPwI)
- took ambient recording
- 2000 Hz high quality recordings
- 5000 Hz poor quality recording

----
## Sources of Issue

- None to think of

----
## Notable Results

![[PhaseAnalysis.png]]
----
## Conclusion

- Looks like there is constantish phase between two channels



