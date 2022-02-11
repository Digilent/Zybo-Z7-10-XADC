Zybo Z7-10 XADC Demo
==============
  
**Note:** The demo contained in this repository has been moved and this repository is no longer being actively maintained. Check out the [Zybo Z7 XADC demo](https://digilent.com/reference/programmable-logic/zybo-z7/demos/xadc) page on Digilent Reference for more information.

Description
--------------
This project is a Vivado demo using the Zybo Z7-10 analog-to-digital converter ciruitry and LEDs, written in Verilog. When programmed onto the board, voltage levels between 0 and 1 Volt are read off of the JXADC header. Each XADC channel will control the brightness of an LED as shown in the following table. See the Zybo Z7-10's [Reference Manual](https://reference.digilentinc.com/reference/programmable-logic/zybo-z7/reference-manual) for more information about how the ZYNQ FPGA's XADC is connected to header JXADC.

| XADC Channel | JXADC Pins             | LED #        | 
| ------------ | ---------------------- | ------------ | 
| AD14         | JXADC1(P) / JXADC7(N)  | LD0          | 
| AD7          | JXADC2(P) / JXADC8(N)  | LD1          | 
| AD15         | JXADC3(P) / JXADC9(N)  | LD2          | 
| AD6          | JXADC4(P) / JXADC10(N) | LD3          | 
  
Requirements
--------------
* **Zybo Z7-10**: To purchase a Zybo Z7-10, see the [Digilent Store](https://store.digilentinc.com/zybo-z7-zynq-7000-arm-fpga-soc-development-board/)
* **Vivado 2018.2 Installation**: To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **MicroUSB Cable**
* **Wires and a Circuit to Measure**

Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Zybo-Z7-10-XADC/releases).
2. Open the project in Vivado 2018.2 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Zybo-Z7-10-XADC.xpr".
3. In the Flow Navigator panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug the Zybo Z7-10 into the computer using a MicroUSB cable.
5. In the green bar at the top of the window, click **Open target**. Select "Auto connect" from the drop down menu.
6. In the green bar at the top of the window, click **Program device**.
7. In the Program Device Wizard, enter "\<archive extracted location\>vivado_proj/Zybo-Z7-10-XADC.runs/impl_1/top.bit" into the "Bitstream file" field. Then click **Program**.
8. The demo will now be programmed onto the Zybo Z7-10. See the Introduction section of this README for a description of how this demo works.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project.

Check out the Zybo Z7-10's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/zybo-z7/start) to find more documentation, demos, and tutorials.

For technical support or questions, please post on the [Digilent Forum](https://forum.digilentinc.com).

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)1
