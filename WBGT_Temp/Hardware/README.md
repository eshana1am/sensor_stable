# Sensor assembly procedures
This document details the procedures used to build a Wet Bulb Globe Temperature Sensor Assembly. 


# Stage 1 - Preparing the PCB

Create two 8-pin female headers and one 2-pin header for connecting the microcontroller to the PCB
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_headers_unconnected.png" width="50%">
</p>

Insert the headers into the corresponding holes as shown and flip over the board for soldering.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_header_soldering.png" width="50%">
</p>

Insert a 2-pin JST connector in the "BAT IN" location for a battery and a switch into the switch position and solder.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_jst_switch.png" width="50%">
</p>

Flip over the board and solder (you may need to tape these components to the board).
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_jst_switch_solder.png" width="50%">
</p>

Locate five 2-pin terminals for the "thermistor", "BAT OUT, and I2C Connections.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_terminals.png" width="50%">
</p>

Insert each terminal into all the labelled locations shown, with the openings facing the text on the PCB, flip over and solder.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_terminal_solder.png"  width="50%">
</p>

Find a 10K-ohm resistor to solder into the remaining non-labelled position as shown and solder after trimming excess leads
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_10k_ohm.png" width="50%">
</p>




# Stage 2 - prepare the MCU

Create two 8-pin male headers and one 2-pin male header for soldering onto the MCU
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_mcu_headers.png" width="50%">
</p>

Insert the 8-pin male headers into the bottom 8 positions of the MCU on each side ("Vin" through "GPIO7" and "VS" through "GPIO10") and Insert the 2-pin header into the "~3" and "~2" As Shown below. 
Confirm the correct positions by referring to the image below.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_mcu_headers_in_place.png" width="50%">
</p>


Then, insert the pins into a breadboard for ease of soldering. Ensure the pins are flush with the MCU and solder all.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_mcu_headers_solder.png" width="50%">


Insert the MCU into the PCB board and ensure the correct pins are connected.
<p align="center">
<img src="../../img/WBGT_Temp/wbgt_mcu_on_board.png" width="50%">





# Stage 3 - battery assembly
With the PCB switch to the "off" position, remove the MCU and attach a 400 mAh battery to the "BAT IN" port.
<p align="center">
<img src="../../img/HTCC-AB02/pcb_w_battery.jpeg" width="50%">
</p>

Insert a 2-pin JST connector into the MCU and add a 2 character board label for MCU identification.
<p align="center">
<img src="../../img/HTCC-AB02/MCU_cable.jpeg" width="50%">
</p>

Insert the other end of the JST connector into the "BAT OUT" port. Ensure the RED wire goes into "VB" and the BLACK wire goes into "G".
<p align="center">
<img src="../../img/HTCC-AB02/MCU_power_pcb.jpeg" width="50%">
</p>

Reinsert the MCU into the PCB, ensure you do not damage the battery. There should be plenty of space between the MCU and the battery if inserted correctly.
<p align="center">
<img src="../../img/HTCC-AB02/Battery_inplace.jpeg" width="50%">
</p>

To test power, move the switch to the ON position. If no sketch has been uploaded to the board, it should flash RGB Testing on the LCD screen, along with different lights, then show the text below. 
<p align="center">
<img src="../../img/HTCC-AB02/Testing_power.jpeg" width="50%">
</p>

Turn off power by moving the switch back to the OFF position.



# Stage 4 - Housing Preparation

<p align="center">
<img src="../../img/ML22F/enclosure.jpeg" width="100%">
</p>

There are a total of 11 parts that need to be 3D Printed, as shown above with preferably ASA type UV Resistant Filament
These Include:
    - Bottom Lid Piece with Mounting and Water Drain X 1 
    - Bottom PCB Housing Plate X 1
    - Middle Plates with Hollow Center Cutout X 4
    - Top Plates with Solid Infill X 2 
    - Top Mounting Piece x 1
    - Top Mount with 1/2" NPT Thread & Solar Panel Mount x 1
    - Sensor Module Mounting Piece x 1

All can be printed without supports but a brim is recommended for better print stability. For better quality overall, a printer with an enclosure or a higher heat environment and dehumidification is recommended for printing with ASA Filament
 
<p align="center">
<img src="../../img/ML22F/enclosure_w_bit.jpeg" width="50%">
</p>

Additionally, the following hardware is also needed. These can be found on McMaster-Carr 
    - 6" 8-32 Stainless Steel 18-8 Threaded Rods X 3 (McMaster 95412A821)
    - 8-32 Nylon 6-6 Wingnut X 6 (McMaster 94924A009)
    - 1/2" NPT Standard Male-Female PVC Connector X 2 (McMaster 4880K61)
    - Small #3  Screws X 2 (no more than 1/8" in length)
    - 1/2" NPT Gland 
    - 1/2" PVC Pipe cut to approx. 6" in length or less
    - Hollow Aluminum sphere which can be spray painted black 


<p>
<img src="../../img/ML22F/hole_in_top.jpeg" width="45%">
<img src="../../img/ML22F/sensor_in_top.jpeg" width="45%">
</p>

Start by 3D Printing the Bottom Lid with Mounting, the top mounting, the solar panel mount, and the Sensor Module Mounting all at 50% Infill Density. 
These can be printed with PLA but ASA is recommended to better resist UV deformation and warping. 

<p align="center">
<img src="../../img/ML22F/antenna_hole.jpeg" width="50%">
</p>

Continue by Printing the Bottom PCB Housing at 50% Infill Density. 
This should be done with ASA 

<p align="center">
<img src="../../img/ML22F/gland_hole.jpeg" width="50%">
</p>

Print 4 Middle Plates with center cutouts at 50% Infill Density also with ASA.

<p align="center">
<img src="../../img/ML22F/gland_in_enclosure.jpeg" width="50%">
</p>

Finally, Print 2 top plates that don't have a central cutout. 
These must be printed with ASA at a 100% Infill Desnity 

<p align="center">
<img src="../../img/ML22F/antenna_connector_in_enclosure.jpeg" width="50%">
</p>

To prepare the black Globe, drill/cut a 1/2" hole into an aluminum sphere 
Once Drilling is done, spray paint the globe black using any matte black spray paint 
<p align="center">
<img src="../../img/ML22F/antenna_connector_in_enclosure.jpeg" width="50%">
</p>

Once the Sphere is dry, it can be bonded to the male end of a 1/2" NPT Connector

<p align="center">
<img src="../../img/ML22F/antenna_connector_in_enclosure.jpeg" width="50%">
</p>

Cut a 1/2" PVC Pipe down to no more than 6" in length.
Push the remaining NPT connector Female end and the connector bonded to the globe onto the pipe 

# Stage 5 - Preparing the Sensors and Solar Panel 

The Sensors Needed are the SHT-45 Sensor and a simple thermistor, but a BME280 or any other temperature I2C compatible will work, as shown below.
A solar panel for recharging the battery is also needed 
4-conductor and 2-conductor cables are needed for the assembly

<p align="center">
<img src="../../img/US-Sensor/soldering_sensor.jpeg" width="50%">
</p>

Begin by soldering stripping the 4-conductor cable 
Solder two of the wires/conductors to the "VIN" Positive and "GND" Ground Pins 
Make note of what color wire each pin is connected to 

<p align="center">
<img src="../../img/US-Sensor/sensor_soldered.jpeg" width="50%">
</p>

Solder the remaining set of conductors for the "SCL" and "SDA" Wires for the I2C 
Make note of these colors as well.
Keep a generous amount of excess cable for final assembly
<p align="center">
<img src="../../img/US-Sensor/gaskets.jpeg" width="50%">
</p>

Next, take a 2-conductor cable, strip it, and solder each wire to the thermistor
The colors/poles of these are negligible
Keep a generous amount of excess cable for final assembly


<p align="center">
<img src="../../img/ML22F/housing_on_sensor.jpeg" width="50%">
</p>

Using another 2-conductor cable, solder the positive and negative pads of the solar panel with generous solder
Keep a generous amount of excess cable for final assembly
<p align="center">
<img src="../../img/HTCC-AB02/sensor_connected.jpeg" width="50%">
</p>


# Interlude - set up software

If you have not done so already, this is a good time to set up the TTN connection and flash the software to the MCU. Follow the instructions [here](../Firmware/README.md).


# Stage 6 - Mount the Electronics 
For Final Assembly, use the hardware as metioned before 

<p align="center">
<img src="../../img/HTCC-AB02/attach_antenna_cable.jpeg" width="50%">
</p>

Screw in the PCB with MCU using #3 screws in the bottom PCB Holding plate and secure

<p align="center">
<img src="../../img/HTCC-AB02/insert_MCU.jpeg" width="50%">
</p>

Remove support material on the bottom Lid mount and thread a 1/4" NPT Cable gland through the corresponding hole as shown
The plastic nut for the gland should be in the recessed area on the inside of the plate as shown

<p>
<img src="../../img/HTCC-AB02/secure_MCU.jpeg" width="45%">
<img src="../../img/HTCC-AB02/MCU_secured.jpeg" width="45%">
</p>

Thread the cables for the I2C temperature sensor, thermistor, and solar panel through the gland
Ensure that the cables are threaded through as shown 
<p align="center">
<img src="../../img/HTCC-AB02/attach_antenna.jpeg" width="50%">
</p>

Connect the Positive and negative wires from the sensor's "VIN" and "GND" pins respectively into the "V+" And "G" labelled terminals on the PCB 

<p align="center">
<img src="../../img/firmware/RSSI.png" width="100%">
</p>

Connect the SCL and SDA wires from the sensor's "SCL" and "SDA" pins respectively into the labelled terminals on the PCB 
<p align="center">
<img src="../../img/firmware/RSSI.png" width="100%">
</p>

Connect the positive and negative wires from the solarpanel into the "VS" and "G" Solar terminals respectively 
<p align="center">
<img src="../../img/firmware/RSSI.png" width="100%">
</p>

Connect both wires to the thermistor terminal as shown. Wire colors/polarity does not matter in this case
<p align="center">
<img src="../../img/firmware/RSSI.png" width="100%">
</p>



# Stage 7 - Full Assembly of Housing 

Solder wire leads onto the back of the solar panel

<p align="center">
<img src="../../img/solar-panel/solar_solder.jpeg" width="50%">
</p>

Using a multimeter, test the voltage coming through the wire leads. With lab lighting and the panel pointing generally at the lights, you should read at least 1 v.

<p align="center">
<img src="../../img/solar-panel/solar_panel_test.jpeg" width="50%">
</p>

Add a generous amount of RTV to the connection to prevent water damage. Seal all electrical connections.

<p align="center">
<img src="../../img/solar-panel/solar_rtv.jpeg" width="50%">
</p>

Apply epoxy to the angled part of the solar panel stand and press firmly onto the solar panel as shown below. Let set overnight.

<p>
<img src="../../img/solar-panel/stand_epoxy.jpeg" width="45%">
<img src="../../img/solar-panel/solar_stand.jpeg" width="45%">
</p>

Once epoxy and RTV are set, thread the wire leads through the gland and connect the V+ wire to the Vs terminal and the V- wire to the G terminal.

<p>
<img src="../../img/HTCC-AB02/solar_connect_leads.jpeg" width="45%">
<img src="../../img/HTCC-AB02/solar_connected.jpeg" width="45%">
</p>

Test the voltage coming from the solar panel on the solar terminal as well as the Vs and Gnd pins of the MCU. If all connections are correct, the voltage should read at least 1 v as before.

<p align="center">
<img src="../../img/solar-panel/solar_test.jpeg" width="50%">
</p>

# Stage 8 - close up and mount sensor

Flatten and twist the sensor wires so they will not be in the way of any components when the cover is on. Close the cover, ensuring no wires are in between the housing and cover. Fasten four screws tightly.

<p align="center">
<img src="../../img/ML22F/close_cover.jpeg" width="50%">
</p>

Tighten gland around cable to ensure no water infiltration is possible.

<p align="center">
<img src="../../img/general/tighten_gland.jpeg" width="50%">
</p>

Add a label to both sides of the sensor housing.

<p align="center">
<img src="../../img/general/label.jpeg" width="50%">
</p>

Locate 2 mount plates and 4 6/32 screws.

<p align="center">
<img src="../../img/general/mount.jpeg" width="50%">
</p>

With the bubble level holes facing away from the housing, attach the mount plates by threading 2 screws each through the holes in the housing and into the interior threaded holes in the plates. Fasten tightly.

<p>
<img src="../../img/ML22F/mounted.jpeg" width="45%">
<img src="../../img/ML22F/mounted_top.jpeg" width="45%">
</p>
