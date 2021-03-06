<ol start="1">
 <li>
  <h4><a href="https://github.com/mdzakirhussain/Advanced-Physical-Design-using-OpenLane-Sky130/blob/main/README.md#day1--inception-of-open-source-eda-openlane-and-sky130-pdk-1" >Day1 – Inception of open-source EDA, OpenLANE and Sky130 PDK</a></h4>
 </li>
</ol>
<ul>
 <li>
How to talk to computers  </li>
<li>SoC design and OpenLANE  </li>
<li>Starting RISC-V SoC Reference design  </li>
<li>Get familiar to open-source EDA tools
  </li>
</ul>
<ol start="2">
 <li>
<h4><a href="https://github.com/mdzakirhussain/Advanced-Physical-Design-using-OpenLane-Sky130#day-2---understand-importance-of-good-floorplan-vs-bad-floorplan-and-introduction-to-library-cells-1">Day 2 - Understand importance of good floorplan vs bad floorplan and introduction to library cells</a></h4>
 </li>
</ol>
<ul>
 <li>
Chip Floor planning considerations</li>
 <li>Library Binding and Placement</li>
 <li>Cell design and characterization flows</li>
 <li>General timing characterization parameters
 </li>
 </ul>
 <ol start="3">
 <li>
<h4><a href="https://github.com/mdzakirhussain/Advanced-Physical-Design-using-OpenLane-Sky130/blob/main/README.md#day-3---design-and-characterize-one-library-cell-using-magic-layout-tool-and-ngspice-1">Day 3 - Design and characterize one library cell using Magic Layout tool and ngspice</a></h4>
 </li>
</ol>
<ul>
 <li>
Labs for CMOS inverter ngspice simulations </li>
 <li>Inception of Layout – CMOS fabrication process
Sky130 Tech File Labs
  </li>
 </ul>
   <ol start="4">
 <li>
<h4><a href="https://github.com/mdzakirhussain/Advanced-Physical-Design-using-OpenLane-Sky130/blob/main/README.md#day-4---pre-layout-timing-analysis-and-importance-of-good-clock-tree-1">Day 4 - Pre-layout timing analysis and importance of good clock tree</a></h4>
 </li>
</ol>
  <ul>
 <li>
Timing modelling using delay tables </li>
<li>Timing analysis with ideal clocks using openSTA </li>
<li>Clock tree synthesis TritonCTS and signal integrity </li>
<li>Timing analysis with real clocks using openSTA
  </li>
    </ul>
      <ol start="5">
 <li>
<h4>Day 5 - Final steps for RTL2GDS</h4>
  </li>
</ol>
<ul>
 <li>
Routing and design rule check (DRC) </li>
<li>PNR interactive flow tutorial
 </li>
  </ul>

<ol start="1">
 <li>
  <h4>Day1 – Inception of open-source EDA, OpenLANE and Sky130 PDK</h4>
 </li>
</ol>

<img src="day1/1 terminal.JPG">
Fig.1 This is the terminal window.<br/>
<br/><img src="day1/2. go to the working directory.JPG">
Fig.2 In the terminal window being in tools diretory do "ls" to list the files and folders.<br>  
<br/>In the fig.2 we can see two folders.<br>  
<ol>
<li>openlane</li>
 <li>pdks</li>
</ol><br/>
<b>To Launch the tool</b><br/>
<br/><img src="day1/4. openlane terminal.JPG">
<br/>Fig.3, to launch the openlane type the command "make mount"<br/>
<br/><b>Types of PDKs(Process Design Kit)</b><br/>
<br/><img src="day1/5 types of pdks.PNG">
Fig.4 It shows the 3 types of PDKs<br/>
<br/>In the figure 4 it seen that there three types of pdks<br/>
<ol><li>skywater-pdk</li><li>open-pdks</li><li>sky130A</li></ol><br/>
<b>PDK used in this Lab is sky130A</b><br/>
<br/><p>This sky130A pdk contains <b>libs.tech,</b> and <b>libs.ref</b></p>
<img src="day1/6 inside libs.tech.PNG">
<br/>Fig.5 It shows the contents of sky130A and libs.tech<br/>
<br/><img src="day1/7 inside libs.ref.PNG">
<br/>Fig.6 It shows the contents of libs.ref<br/>
<br/><b>The library used from the sky130A pdk is sky130_fd_sc_hd</b><br/>
<br/><img src="day1/8 lib we are working with.PNG">
Fig.7 It shows the contents of sky130_fd_sc_hd<br/>
<br/><b>The sky130_fd_sc_hd contains various process corners, which are shown in the figure below</b><br/>
<br/><img src="day1/9 process corners in the lib.PNG">
Fig. 8 Figure shows the various process corners<br/>
<br/><b>openlane terminal needs to be launched from being in the openlane directory, which is shown in the figure below</b><br/>
<br/><img src="day1/11 invoke openlane terminal from openlane dir.PNG">
<br/>Fig.9 Figure shows oipenlane directory.<br/>
<br/><b>From the openlane directory type the command "make mount"</b><br/>
<br/><img src="day1/12 invoking command.PNG"><br/>
Fig. 10 Figure shows the command "make mount"
<b>To start the flow in interactive way type the way shown in the below figure"</b><br/>
<br/><img src="day1/13 after invoking pre design.PNG"><br/>
Fig.11 Figure shows the command for making the tool interactive.<br/>
<br/><img src="day1/14 after prep.png"><br/>
Fig.12 Figure shows the preparation stage which creates necessary directories.</br>
<h4>To run the synthesis</h4>
<br/><img src="day1/15 run synth.png"><br/>
Fig. 13 Figure shows the synthesis command<br/>
<br/><img src="day1/16 synth1.PNG">
Fig. 14-a Synthesis Results<br/>
<br/><img src="day1/17 synth2.PNG">
Fig. 14-b Synthesis Results<br/>

<br/><img src="day1/18 synth3.PNG"><br/>
<br/>Fig. 14-c Synthesis Results<br/>

<ol start="2">
 <li>
<h4>Day 2 - Understand importance of good floorplan vs bad floorplan and introduction to library cells</h4>
 </li>
</ol>
<h4>To run the floor plan</h4>
<img src="day2/1. run floor plan.png">
Fig. 1 Figure shows the command to run the floorplan
<h4> Visualize the floorplan done in the magic</h4>
<img src="day2/2. to see after floorplan command in magic.png">
Fig. 2 Figure shows the command to visualize the floorplan in the magic tool
<img src="day2/3 floorplanned_1.png">
Fig. 3 Figure shows complete floorplan of the design picorv32a
<img src="day2/4 floorplanned_2 Horizontal io.png">
Fig. 4 Figure shows the horizontal IO
<img src="day2/5 floorplanned_3 vertical io.png">
Fig. 5 Figure shows the vertical IO
<img src="day2/6 standard cells after florr plan.png">
Fig. 6 Figure shows the standard cells after floorplan done
<h4>To run the placement</h4>
<img src="day2/7 global placement.png">
Fig. 1 Figure shows the command to run the placement
<img src="day2/8 after placement.png">
Fig. 2 Figure shows the command to visualize the placement in the magic tool
<img src="day2/8 after placement_2.png">
Fig. 3 Figure shows placement done in the magic tool
<br/>
 <ol start="3">
 <li>
<h4>Day 3 - Design and characterize one library cell using Magic Layout tool and ngspice</h4>
 </li>
</ol>
<img src="day3/1 setting io pins distance.png">
Fig. 1 Figure shows IO pins setting
<img src="day3/2 after setting pins run floorplan again.png">
Fig. 2 Figure shows the command to run floorplan after setting IO distance
<img src="day3/3 foorplan in magic.png">
Fig. 3 Figure shows the command to see in the magic tool after fllorplan is done
<img src="day3/4 pins are not placed equally.png">
Fig. 4 Figure shows PINS are not equidistance 
<img src="day3/5 inverter cell.png">
Fig. 5 Figure shows the command to open the inverter in the magic tool
<img src="day3/7 inverter spice netlist.png">
Fig. 6 Figure shows the spice netlist generated by the magic tool
<img src="day3/8 inverter simulation.png">
Fig. 7 Figure shows the simulation done using ngspice for the inverter design
<br/>
<ol start="4">
 <li>
<h4>Day 4 - Pre-layout timing analysis and importance of good clock tree</h4>
 </li>
</ol>
<img src="day4/1 invoke magic for inverter design.png">
Fig.1 Figure shows the inverter design in the magic tool
<img src="day4/2 layout inverter.png">
Fig. 2 Figure shows the layout of the design in the magic tool
<img src="day4/3 grid command.png">
Fig. 3 Figure shows the grid command, it is for the purpose of creating LEF file
<img src="day4/4 step1 label to port.png">
Fig. 4-1 Figure shows the process to convert Labels to Ports
<img src="day4/5 step2.png">
Fig. 4-2 Figure shows the process to convert Labels to Ports
<img src="day4/6 lef file.png">
Fig. 5 Command to generate LEF file
<img src="day4/7 edit config dot tcl file.png">
Fig. 6 Figure shows editing of the config dot tcl file to run the custom built cells
<img src="day4/8 files required in src folder.png">
Fig. 7 Figure shows the required files that are required in the src folder of the design
<img src="day4/9 prepare the design.png">
Fig. 8 Figure shows the design preparation for synthesis and other steps
<img src="day4/10 after placement and routing read in magic.png">
Fig. 9 Figure shows the placed logic in the magic layout tool
<img src="day4/11 routed.png">
Fig. 10 Figure shows the routed design
<img src="day4/12 custom cell.png">
Fig. 11 Figure shows our custom cell
