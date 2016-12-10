# RR-CANMAN-CCN01
This is an effort to reverse engineer the CANMAN CCN01 eeprom, the goal is to create a working bin file for a reset module specifically for the Startboard side Jet installed in M/Y Sunglider ii

The target bin file output is a copy of the CANMAN ID21(working module).bin with a node id of 24 and node name of SO-Master instead.(Starboard side Jet Master)

CANMAN ID21(working dump).bin is the EEPROM dump of the CCN01 module with node id of 21 and node name of PO-Master (Port side Jet Master)

CANMAN ID25(working dump).bin is the EEPROM dump of the CCN01 module with node id of 25 and node name of CT-Master (Center Jet Master)

CANMAN CCN01 RESTORED BLANK.bin is the EEPROM dump generated from blank EEPROM installed on CCN01 board and powered up with the Restore dip switch switched on.

Here's a nice reference for this project: http://www.es.mdh.se/pdf_publications/486.pdf a masters thesis of Mr. Anders Möller of Mälardalen University, Sweden
