# AxisControl

## What is this repository for? ##

* AxisControl program in Beckhoff TwinCAT 3.1
* A sample PLC program that provides an axis object filled with controlling methods, useful for testing axes quickly

## How do I get set up? ##

+ Minimum requirements (as tested) 
	* Visual Studio 2019
    * ------- OR -------
    * TwinCAT XAE Shell 3.1.4024.56

## How do I use this? ##

* AxisControl function block has an AXIS_REF that needs to be linked to an NC axis. Once this link has been made inside of the NC, the methods can be called to control the axis. The function block does not need to be called directly
* Calling CyclicUpdate() every cycle is required. This method updates the internal state of the function block
* Include Tc2_Mc2 library for access to MC function blocks that are used internally

## Who do I talk to? ##

* Beckhoff UK - Ben Sturdy