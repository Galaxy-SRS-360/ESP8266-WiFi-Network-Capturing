# ESP8266 WiFi Captive 

## Disclaimer
This project is for testing and educational purposes. Use it only against your own networks and devices. I don't take any responsibility for what you do with this program.

## About this project
WiFi captive  for the NodeMCU (ESP8266 Module) with DNS spoofing.

The built-in LED will blink 5 times when a password is posted.

<b>Warning!</b> Your saved passwords will **not** disappear when you restart/power off the ESP8266.

<b>Note:</b> If you want to see the stored passwords go to "**192.168.6.21**<a>/pass</a>". For changing the SSID, go to "**192.168.6.21**<a>/ssid</a>"


# Screenshots

<table>
  <tr>
    <th>192.168.6.21/index</th>
    <th>192.168.6.21/post</th> 
    <th>192.168.6.21pass</th>
    <th>192.168.6.21ssid</th>
  </tr>
  <tr>
    <td>This is the main page. Here the user will write his password and send it.</td>
    <td>This is the post page. The user will be redirected here after posting the password.</td>
    <td>This is where the attacker can retrieve all the passwords that has been posted.</td>
    <td>Here the attacker can change the SSID name of the Access Point on the go.</td>
  <tr>
    <td><img width="200px" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal/master/src/1_Index_2.jpg" title="index"></td>
    <td><img width="200px" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal/master/src/2_Post.jpg" title="post"></td>
    <td><img width="200px" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal/master/src/3_Pass.jpg" title="pass"></td>
<td><img width="200px" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal/master/src/4_ssid.jpg" title="ssid"></td>
  </tr>
</table>

# Installation (ESP8266 Flasher - Easy way)

1. Download <a href="https://github.com/nodemcu/nodemcu-flasher"><b>ESP8266 Flasher</b></a>.

2. Download the <b><a href="https://github.com/125K/ESP8266_WiFi_Captive_Portal/releases/download/1.1/release.bin">release.bin</b></a> file.

3. Open the ESP8266 Flasher and select the Node MCU port

<img width="80%" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/1_port_selection.PNG">

4. Then, go to the config tab and select the .bin file you've just downloaded.

<img width="80%" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/2_file_selection.png">

5. Finally, go back to the first tab and press "Flash"

6. Your Node MCU is ready!

# Installation (Arduino IDE)

1. Open your <a href="https://www.arduino.cc/en/main/software">Arduino IDE</a> and go to "File -> Preferences -> Boards Manager URLs" and paste the following link:
``http://arduino.esp8266.com/stable/package_esp8266com_index.json``
2. Go to "Tools -> Board -> Boards Manager", search "esp8266" and install esp8266
3. Go to "Tools -> Board" and select you board"
4. Download and open the sketch "<a href="https://github.com/Galaxy-SRS-360/ESP8266-WiFi-Network-Capturing/blob/main/WiFi_Captive.ino"><b>WiFi_Captive.ino</b></a>"
5. You can optionally change some parameters like the SSID name and texts of the page like title, subtitle, text body...
6. Upload the code into your board.
7. You are done!



