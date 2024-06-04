# WeatherPico
Weather station using a Raspberry Pi pico w, pico and (mainly) another machine.<br>
<br>
It uses the PiicoDev modules by Core Electronics to transmit between the weather station outside node and the receiver node (the Pico W). <br>
<br>
# Installaton
You will requrire the following hardware:
<ul>
<li>Raspberry Pi Pico and Raspberry Pi Pico W</li>
<li>If Pico W does not have headers, use stackable headers.</li>
<li>Waveshare 1.8" screen</li>
<li>If not using stackable headers, a QUAD EXPANDER for picos</li>
<li>PiicoDev BME280 Temperature Sensor</li>
<li>PiicoDev 915MHz transceiver (2)</li>
<li>PiicoDev Expansion board for Pico</li>
<li>200mm Cables for PiicoDev appliances. 
<li>Optional: third machine that does not run micropython (like a NUC or Raspberry Pi 3/3B/3B+/4/5)</li>
<li>Optional: Micro:Bit for a secondary sensor.</li>
</ul><br>
These are all buyable at <a href="https://core-electronics.com.au">Core electronics AU</a>

### Setup

<ol>
  <li>Using the quad expander or stackable headers, connect the display and expansion board to the pico w. If using the stackable headers, make sure the screen is at the top as it is a non-stackable module.</li>
  <li>Using <a href="">This MicroPython image</a>, flash it onto the pico w. Flash <a href="">This image</a> to the Pico. These images do not contain the packages pre-installed. </li>
  <li>Using Thonny, upload the code and the requirements.txt file (from this repo) to the Pico. Upload the files in the Pico_W folder to the Pico W and upload the files in the Pico folder to the Pico.</li>
  <li>In Thonny, Go to Tools > Manage packages and click on the button that allows you to install from a requirements.txt file. Use the respective requirements.txt files for each machine.</li>
  <li>Connect the Pico modules using the PiicoDev cables. Make sure you use the longer ones as you probably want to.</li>
  <li>If you want to run this code without needed a webserver, download the other main.py in the NoServer directory in the Pico_W folder.</li>
  <li>Start and enjoy. Make sure the Pico is transmitting the weather or the display will not update.</li>
</ol>
