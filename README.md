## Fork from OE3CJB
This is forked from OE3CJB at 01.03.2021

Look here for his comments an repository
https://github.com/oe3cjb/TTGO-T-Beam-LoRa-APRS


I forked it for my preparing private versions relying on his and others ideas. 

If you want to discuss with other LoRa APRS interested persons join the growing community at the LoRa-APRS Telegram group

## Remark
In Hannover we have some trouble with the compressed tracker mode. Some RPi+GWHat confiogurations stop working after some time if "flooded" with compressd data.
We will investigate the reasons

Therefore compression  
 define TX_BASE91
in line 240 of ../src/TTGO_T-Beam_LoRa_APRS.ino is commented out.


## Intention
I forked this version because of my intention to build a specialized tracker for my mobile home. It should collect data from some sensors, weather condition etc. and send it to the APRS-System in two ways: If no wifi is present, it should just send the Packet to 433 MHz. If a known wifi is present, it should try to send the packet via wifi to the APRS-System direct.



# Future plans

* [ ] add sending packet direct via wifi to aprs-net (using work from Peter, OE5BPA)
* [ ] some refactoring
* [ ] REST-API or communication with webserver
* [ ] web-page sensors information
* [ ] etc.
