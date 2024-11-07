# MOTHER BOARD SPECS
Started Oct 23, 2024

## Mechanical Specs
**Av Bay Dimensions |**
[CubeSat] specification:
- Width-Max: 10cm
- Depth-Max: 10cm
- Height-Max: max sub-board length, 10cm ?

**Mother Board Dimensions:**
- Width: 10cm
- Height: 10cm?
- 2x2cm cut outs from corners


## Connector Specs
- D'sub connectors 
- MAKE IT BIG, LIKE 10CM (structural)
- Protocol standard for each pin
- 90° Connectors from mother board, Parallel connectors on sub boards

## Power Specs
**12V, 5V, 3V3?** Wire gauge, Amp max

**Current Draw:** 
- 2A, 3V3 (radio)
- WHAT DO THE OTHER BOARDS NEED???

**Chassis Ground???**
- Depends on what material the chassis is made of 


## Data Line Specs
### CAN Bus
The can bus protocal runs through the board top to bottom.
And is daisy chained at top and bottom

Maximum signaling rate of 1 megabit per second (bps). 120Ω terminating resistance

### Dirrect Camera Data Lines:
Maybe if we have radio bandwidth

**RSB:** UART (~5Mbs)?

### Connector Pin Assigments:
What are the connector pins assigned to? Gotta figure out what power requirement look like before asignment can be made.

## Sub-Board List
- [DBC](#daughter-board-cube-dbc) RSB Radio Board (Ana)
- Camera Board??
- [DBC](#daughter-board-cube-dbc) Flight Control Board FCB (El-Mougey)
- [DBC](#daughter-board-cube-dbc) Camera Interface Board CIB ()
- [SAC](#sensor-and-actuator-cube-sac) Data Aquisition DAQ (Rhoda)
- [PC](#power-cube-pc) Battery Management Board BMS ()
- [PC](#power-cube-pc) Power Management Board PMB


## CubeSats We Need:
### Power Cube (PC): 
- Contains bateries and BMS and PMB. 
- *Raw Battery Power Never Touches the MotherBoard* 
- BMS will connect to mother board for DAQ
- PMB connects to mother board to supply power

### Daughter Board Cube (DBC):
- Contains standard Ave bay PCBs
- Any number of these may be used based on number of PCBs

### Sensor and Actuator Cube (SAC):
- DAQ board lives here (has sensors connected)
- Actuator board
- Wall mount connectors for all sensor connectors (Patch/GPS intena included)


## TODO
- Pick connectors daughter board and mother board daisy chain
- Pick connectors for wall mount connectors sensors (Rhoda + Mohammad)
- Find total current draw
- Determine how terminating resistors work with daisy chain
- CAD the SatCube Structure






[CubeSat]: https://en.wikipedia.org/wiki/CubeSat