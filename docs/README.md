![[Overview.drawio.svg]]

The board is to be inserted in the Slot1 and Slot2 of a 6-Slot Crate with a triplicated mesh fabric,  
in this way we can loopback all channels that would be present when we have a node board (Serenity) inserted in the Slots 3,4,5,6 of this crate as if it would be on a regular 14 slot dual-fabric.  

The simple loopback card will forward the base channels to a RJ45 connector with included magnetics,    
and each fabric channel would have the TCDS2, 10GbE, TTC/TTS channels in loopback with the exception of slot 4 which is meant to receive TCDS2 from a fiber link, similar to 10GbE. In this way, a board at the factory needing testing can have one slot in the back and two slots in the front that could be empty.

A first idea implemented only passive components breaking out the clocks in a pairs of MMCX (space reasons), however in another thought there is the possibility to include a PLL do distribute the clocks, this however require that an isolated 3V3 DC-DC converter is included to provide power to the active components like the PLL.


![[6_Slot_Crate.png]]
[ref](https://schroff.nvent.com/sites/g/files/hdkjer281/files/acquiadam/2020-11/63972-317.pdf)




![[14_Slot_Crate.png]]
[ref](https://catalogue.library.cern/literature/5p184-jtb90)

