# Rolls-Royce CANMAN-CCN01
This is an effort to reverse engineer the Rolls-Royce CANMAN CCN01 eeprom, the goal is to create a working bin file for a reset module specifically for the Startboard side Jet installed in M/Y Sunglider ii

The target bin file output is a copy of the CANMAN ID21(working module).bin with a node id of 24 and node name of SO-Master instead.(Starboard side Jet Master)

CANMAN ID21(working dump).bin is the EEPROM dump of the CCN01 module with node id of 21 and node name of PO-Master (Port side Jet Master)

CANMAN ID25(working dump).bin is the EEPROM dump of the CCN01 module with node id of 25 and node name of CT-Master (Center Jet Master)

CANMAN CCN01 RESTORED BLANK.bin is the EEPROM dump generated from blank EEPROM installed on CCN01 board and powered up with the Restore dip switch switched on.

Here's a nice reference for this project: http://www.es.mdh.se/pdf_publications/486.pdf a masters thesis of Mr. Anders Möller of Mälardalen University, Sweden

# Update (December 11, 2016 2:50AM GMT+8)

for the CANMAN ID21(working dump).bin and CANMAN ID25(working dump).bin the node ID is stored at EEPROM address 3A7 followed by it's single byte CRC (3A8) as of this time, i really haven't figured out how the CRC byte is calculated, but i tried copying the node id and the crc byte to the other bin file and it works.
