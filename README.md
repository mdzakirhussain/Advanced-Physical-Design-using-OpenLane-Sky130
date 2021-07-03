<h2><p align="center">Advanced Physical Design using OpenLANE/Sky130</p><p align="center">5-Day online mode workshop</p><p align="center">By</p><p align="center">VLSI System Design, Banglore, India.</p></h2>

<h3>Workshop Day wise Content :</h3>
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
<h4>Day 2 - Understand importance of good floorplan vs bad floorplan and introduction to library cells</h4>
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
<h4>Day 3 - Design and characterize one library cell using Magic Layout tool and ngspice</h4>
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
<h4>Day 4 - Pre-layout timing analysis and importance of good clock tree</h4>
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
<br/><img src="day1/15 run synth.png"><br/>
Fig. 13 Figure shows the synthesis command<br/>
<br/><img src="day1/16 synth1.PNG">
Fig. 14-a Synthesis Results<br/>
<br/><img src="day1/17 synth2.PNG">
Fig. 14-b Synthesis Results<br/>

<br/><img src="day1/18 synth3.PNG"><br/>
<br/>Fig. 14-c Synthesis Results<br/>



