
# Guide to simulate PLC and HMI Communication over Modbus TCP

  - [1. Engineering Tools Download](#download-softwares)
  - [2. PLC Project](#plc-project)
  - [3. HMI Project](#hmi-project)

<a id="download-softwares"> </a>

## 1. Engineering Tools Downloads

Download and install the PLC software EcoStruxure Machine Expert Basic [here] and the HMI software EcoStruxure Vijeo Designer Basic [here]. The currently sample project supports Machine Expert Basic version 1.2 SP1 Patch 1 build 65760 and Vijeo Designer Basic V2.0.0.48.

<a id="plc-project"> </a>
## 2. PLC Project

Download the sample PLC project [here], unzip and open (Ctrl+O) the file.
The project has the following Modbus address characteristics:

* Read Coils:  The sample has Modbus Coils addresses 01 to 06 mapped to sequential blinkers, the coils will blink each second in sequential order.
* Read Holding Registers:  Modbus Registers 40001 to 40006 are mapped to counters, and they have the following ranges: 40001 [0:100], 40002 [100:200], 40003 [300:400], 40005 [500:600] and 40006 [500:700].
* Read/Write Coils:  Modbus Coils addresses 101 to 106 are not mapped to any value, so the HMI can toggle them and read back.
* Read/Write Holding Registers:  Modbus Registers 40101 to 40106 are not mapped to any values, the HMI can write them and read back.

The simulation opens the local 502 port for Modbus TCP communication. To start the PLC simulation follow the steps below:

![](images/plc_simulation.png)

1. Click on Simulator Icon or enter Ctrl+B to Lauch Simulator.
2. Click on Play Icon or enter Ctrl+M to Start PLC.


<a id="hmi-project"> </a>
## 3. HMI Project

Download the sample HMI project [here], unzip and import following the steps below:

![](images/hmi_import.png)

1. Click to cancel the Welcome Screen.
2. **Right Click** Vijeo-Manager item on Navigator tool.
3. CLick on Import Project.
4. Select the sample project.
5. Click to enable Open Project After Import.
6. Open the project.
   

