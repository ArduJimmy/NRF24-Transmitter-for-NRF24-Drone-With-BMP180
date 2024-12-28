# UPGRADING NRF24 QUADX TRANSMITTER for NRF24 Multiwii DRONE 2.3 with BMP180

<h2>This project ONLY WORKS for LADYBIRD Board Type with Custom Multiwii 2.3</h2>
<p><b>Disclaimer:</b> If you take this project, you agree that you take your own risk. Please be careful. Safety is always number #1</p>

<h2>UPGRADED NRF24L01 TRANSMITTER <br />FOR NRF24L01 MINI QUADCOPTER + MULTIWII 2.3 + BMP180</h2>
<p>In this project, I add a Trimmer feature, including: 2 buttons for ROLL and 2 buttons for PITCH. All is integrated in Standard NRF24L01 Transmitter. Please see our Videos listed below:</p>

<ol>
  <li><a href="https://www.youtube.com/watch?v=4M9A6sWJjzM" target="_blank">How to make Standard NRF24L01 Transmitter</a></li>
  <li><a href="https://www.youtube.com/watch?v=yUBT2pSCmG8" target="_blank">How to Instal & Activate Altitude Hold on NRF24L01 Quadcopter</a></li>
  <li><a href="https://www.youtube.com/watch?v=wbK7oOLr6PM" target="_blank">How to make NRF24L01 Quadcopter + Multiwii 2.3</a></li>
  <li><a href="https://www.youtube.com/watch?v=FOICuyzBk54" target="_blank">Flying Test: NRF24L01 Mini Quadcopter</a></li>
  <li><a href="https://www.youtube.com/watch?v=sLL9Ln12AQs" target="_blank">Main Troubleshooting Tips with NRF24L01</a></li>  
  <li><a href="" target="_blank">Upgrading NRF24 Transmitter for NRF24L01 with Trimmers</a></li>
  <li>Flying Demo: How To train your drone on Hover (will be available soon)</li>  
</ol>

<p>All those videos are related each other. I'm so glad to share those all to you for free without hidden tips, tricks or else. </p>

<h3>PIN CONFIGURATION</h3>
<p>Please take notice carefully all pins wiring below. This wiring is only for upgraded NRF24 Transmitter for <b>NRF24 Drone with BMP180 ONLY!</b>. You can choose one of this following pin configurations based on your NEED!</p>

<h4>SPECIFIC JOYSTICK + LCD ONLY + Trimmers</h4>
<ul>
  <li>D4 Arduino to CE pin of NRF24L01</li>
  <li>D3 Arduino to CSN  pin of NRF24L01</li>
  <li>D13 Arduino to SCK pin of NRF24L01</li>
  <li>D11 Arduino to MOSI pin of NRF24L01</li>
  <li>D12 Arduino to MISO pin of NRF24L01</li>
  <li>VCC and GND input pins of NRF24-Breakout to VCC and GND pins of Arduino</li>
  <li>VCC pins of Specific Joystick to VCC pin of Arduno</li>
  <li>GND pins of Specific Joystick to GND pin of Arduino</li>
  <li>A0 pin of arduino to <b>X-AXIS</b> pin of Specific Joystick</li>
  <li>A1 pin of arduino to <b>Y-AXIS</b> pin of Specific Joystick</li>
  <li>A2 pin of arduino to VRY pin of Cheap Joystick or Y-AXIS of Specific Joystick (ROLL)</li>
  <li>A3 pin of arduino to VRX pin of Cheap Joystick or X-AXIS of Specific Joystick (PITCH)</li>
  <li>VCC and GND pins of LCD to VCC and GND pins of Arduino (5v)</li>
  <li>SCL pin of LCD to A5 pin of Arduino</li>
  <li>SDA pin of LCD to A4 pin of Arduino</li>
  <li>AUX1: D9 pin of Arduino to Signal pin of Toggle Switch (we dont use AUX2, AUX3, etc.)</li>
  <li>VCC and GND output pins of Step-up Converter to VCC and GND pins of Arduino</li>
  <li>VCC and GND INPUT pins of Step-up Converter to VCC and GND pins of Battery 18650 3.7v 1200mAh</li>  
  <li>D5 pin of Arduino to Button 1 signal pin (Trimmer for PITCH DOWN)</li>
  <li>D6 pin of Arduino to Button 2 signal pin(Trimmer for PITCH UP)</li>
  <li>D7 pin of Arduino to Button 3 signal pin(Trimmer for ROLL DOWN)</li>
  <li>D8 pin of Arduino to Button 4 signal pin(Trimmer for ROLL UP)</li>
  <li>GND of Button pins to GND of Arduino</li>
</ul>

<h4>CHEAP ANALOG JOYSTICK + LCD ONLY + Trimmers</h4>
<p><b>NOTE:</b> If you use a CHEAP ANALOG JOYSTICK then this transmitter can not be used to train your NRF24 drone to activate Altitude Hold Mood ON</p>
<ul>
  <li>D4 Arduino to CE pin of NRF24L01</li>
  <li>D3 Arduino to CSN  pin of NRF24L01</li>
  <li>D13 Arduino to SCK pin of NRF24L01</li>
  <li>D11 Arduino to MOSI pin of NRF24L01</li>
  <li>D12 Arduino to MISO pin of NRF24L01</li>
  <li>VCC and GND input pins of NRF24-Breakout to VCC and GND pins of Arduino</li>
  <li>VCC pin of Cheap Joystick to VCC pin of Arduno</li>
  <li>GND pin of Cheap Joystick to GND pin of Arduino</li>
  <li>A0 pin of arduino to VRX pin of Cheap Joystick</li>
  <li>A1 pin of arduino to VRY pin of Cheap Joystick</li>
  <li>A2 pin of arduino to VRY pin of Cheap Joystick</li>
  <li>A3 pin of arduino to VRX pin of Cheap Joystick</li>
  <li>VCC and GND pins of LCD to VCC and GND pins of Arduino (5v)</li>
  <li>SCL pin of LCD to A5 pin of Arduino</li>
  <li>SDA pin of LCD to A4 pin of Arduino</li>
  <li>AUX1: D9 pin of Arduino to Signal pin of Toggle Switch (we dont use AUX2, AUX3, etc.)</li>
  <li>VCC and GND output pins of Step-up Converter to VCC and GND pins of Arduino</li>
  <li>VCC and GND INPUT pins of Step-up Converter to VCC and GND pins of Battery 18650 3.7v 1200mAh</li>  
  <li>D5 pin of Arduino to Button 1 signal pin (Trimmer for PITCH DOWN)</li>
  <li>D6 pin of Arduino to Button 2 signal pin(Trimmer for PITCH UP)</li>
  <li>D7 pin of Arduino to Button 3 signal pin(Trimmer for ROLL DOWN)</li>
  <li>D8 pin of Arduino to Button 4 signal pin(Trimmer for ROLL UP)</li>
  <li>GND of Button pins to GND of Arduino</li>
</ul>

<h4>CHEAP ANALOG JOYSTICK + Trimmers</h4>
<p><b>NOTE:</b> If you use a CHEAP ANALOG JOYSTICK then this transmitter can not be used to train your NRF24 drone to activate Altitude Hold Mood ON</p>
<ul>
  <li>D4 Arduino to CE pin of NRF24L01</li>
  <li>D3 Arduino to CSN  pin of NRF24L01</li>
  <li>D13 Arduino to SCK pin of NRF24L01</li>
  <li>D11 Arduino to MOSI pin of NRF24L01</li>
  <li>D12 Arduino to MISO pin of NRF24L01</li>
  <li>VCC and GND input pins of NRF24-Breakout to VCC and GND pins of Arduino</li>
  <li>VCC pin of Cheap Joystick to VCC pin of Arduno</li>
  <li>GND pin of Cheap Joystick to GND pin of Arduino</li>
  <li>A0 pin of arduino to VRX pin of Cheap Joystick</li>
  <li>A1 pin of arduino to VRY pin of Cheap Joystick</li>
  <li>A2 pin of arduino to VRY pin of Cheap Joystick</li>
  <li>A3 pin of arduino to VRX pin of Cheap Joystick</li>
  <li>AUX1: D9 pin of Arduino to Signal pin of Toggle Switch (we dont use AUX2, AUX3, etc.)</li>
  <li>VCC and GND output pins of Step-up Converter to VCC and GND pins of Arduino</li>
  <li>VCC and GND INPUT pins of Step-up Converter to VCC and GND pins of Battery 18650 3.7v 1200mAh</li>  
  <li>D5 pin of Arduino to Button 1 signal pin (Trimmer for PITCH DOWN)</li>
  <li>D6 pin of Arduino to Button 2 signal pin(Trimmer for PITCH UP)</li>
  <li>D7 pin of Arduino to Button 3 signal pin(Trimmer for ROLL DOWN)</li>
  <li>D8 pin of Arduino to Button 4 signal pin(Trimmer for ROLL UP)</li>
  <li>GND of Button pins to GND of Arduino</li>
</ul>

<h4>SPECIFIC JOYSTICK + Trimmers</h4>
<ul>
  <li>D4 Arduino to CE pin of NRF24L01</li>
  <li>D3 Arduino to CSN  pin of NRF24L01</li>
  <li>D13 Arduino to SCK pin of NRF24L01</li>
  <li>D11 Arduino to MOSI pin of NRF24L01</li>
  <li>D12 Arduino to MISO pin of NRF24L01</li>
  <li>VCC and GND input pins of NRF24-Breakout to VCC and GND pins of Arduino</li>
  <li>VCC pins of Specific Joystick to VCC pin of Arduno</li>
  <li>GND pins of Specific Joystick to GND pin of Arduino</li>
  <li>A0 pin of arduino to <b>X-AXIS</b> pin of Specific Joystick</li>
  <li>A1 pin of arduino to <b>Y-AXIS</b> pin of Specific Joystick</li>
  <li>A2 pin of arduino to VRY pin of Cheap Joystick or Y-AXIS of Specific Joystick (ROLL)</li>
  <li>A3 pin of arduino to VRX pin of Cheap Joystick or X-AXIS of Specific Joystick (PITCH)</li>
  <li>AUX1: D9 pin of Arduino to Signal pin of Toggle Switch (we dont use AUX2, AUX3, etc.)</li>
  <li>VCC and GND output pins of Step-up Converter to VCC and GND pins of Arduino</li>
  <li>VCC and GND INPUT pins of Step-up Converter to VCC and GND pins of Battery 18650 3.7v 1200mAh</li>  
  <li>D5 pin of Arduino to Button 1 signal pin (Trimmer for PITCH DOWN)</li>
  <li>D6 pin of Arduino to Button 2 signal pin(Trimmer for PITCH UP)</li>
  <li>D7 pin of Arduino to Button 3 signal pin(Trimmer for ROLL DOWN)</li>
  <li>D8 pin of Arduino to Button 4 signal pin(Trimmer for ROLL UP)</li>
  <li>GND of Button pins to GND of Arduino</li>
</ul>

<h2>FULL SCHEMATIC DIAGRAM FOR SPECIFIC JOYSTICK</h2>
<p>You can replace if you dont need LCD or and want to change it to Cheap Joystick. <b>But, Cheap Joystick can not be used to TRAIN our NRF24 Altitude-Hold Mode Drone!!!!!!</b></p>

<img src="https://github.com/ArduJimmy/NRF24-Transmitter-for-NRF24-Drone-With-BMP180/blob/main/full-schematic-specific-joystick-diagram.jpg" alt="Schematic Diagram for Specific Joystick ONLY" title="Schematic Diagram for Specific Joystick ONLY"/>


<h3>GND Wiring</h3>

<img src="https://github.com/ArduJimmy/NRF24-Transmitter-for-NRF24-Drone-With-BMP180/blob/main/gnd-joystick-wiring.jpg" alt="GND Wiring for Specific Joystick ONLY" title="GND Wiring for Specific Joystick ONLY"/>

<h3>VCC Wiring</h3>

<img src="https://github.com/ArduJimmy/NRF24-Transmitter-for-NRF24-Drone-With-BMP180/blob/main/vcc-joystick-wiring.jpg" alt="VCC Wiring for Specific Joystick ONLY" title="VCC Wiring for Specific Joystick ONLY"/>

<h3>X-AXIS and Y-AXIS Wiring</h3>

<img src="https://github.com/ArduJimmy/NRF24-Transmitter-for-NRF24-Drone-With-BMP180/blob/main/AXIS-joystick-wiring.jpg" alt="X-AXIS and Y-AXIS for Specific Joystick ONLY" title="X-AXIS and Y-AXIS for Specific Joystick ONLY"/>

<h3>HOW TO TRAIN YOUR NRF24L01 Quadcopter to Activate Altitude Hold Mode ON</h3>
<p>The Flying Demo Will be available soon .........</p>


<h4>HOW TO SUPPORT US?</h4>
<p>Please Subscribe and Share our videos if you feel that ours videos are useful for you and others. I want all people know how to make drone!</p>
