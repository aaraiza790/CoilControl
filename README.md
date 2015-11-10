#Coil King
#This is the repository to the current Raspberry Pi Install.
#Current install incorporates iSpresso (www.Ispresso.net -  http://bitbucket.org/veggiebenz/pyspresso.git) repository with modification to the temperate sensor to read the one specifically designed for desired heating element and thermocouple (1-wire “3b” Hardware 1Wire Sensor. )

# This install utilizes the python code to create a web java application that is ran on the RPI and can be fully accessible from devices connected within the Local Area Network (LAN). What is requested, is to turn the Web Java Application into an actual application that can be utilized on a touch screen that is connected to the Raspberry Pi. Example: RPI Touch Screen . And can be fully controlled via Touch, Application or Web Access Via Cloud Server. 
 
#The Application will be fully running on device and will also have an application that will  be download-able on Android and other OS, and can be web accessed. A cloud type server will be created so each Controller will receive its own IP/Port on the server to constantly stay connected (with WIFI access) to receive commands and show consistent updated stats to devices running application or web interface.
#In the event that WIFI will be unreliable or not an option, There will be the touch screen on the device to make the changes or it will also have a blue tooth option to receive commands from devices connected nearby.  
#Repository will have folder with Vague Request for layout of Screen/GUI in JPEG form.

 


#Startup
#Initial startup will ask for:
#1) Profile Name (Possible Option to have multiple profiles per user on device?)
#	Profiles will save: Set Temperatures, Wifi/Bluetooth Connection Options
#	Profiles will also enable Password Lock for Parental/Safety Reasons
#2) Internet Connection Information: Network Name / Network Password
#3) No Wifi Available or once Wifi becomes unavailable, Activate Bluetooth?
#4) Verify Settings in Settings Page. Once Complete, Access to Home Screen.
  
#Home Screen
#Home Screen will Display:
#1) Current Temperature of Thermocouple (Requesting to read thermocouple every .5 Seconds.)
#2) Set Temperature (Requested Temperature thermocouple to reach

#Home Screen Buttons:
#1) Temp Up: Will Raise The Set Temperature Value up one point (Hold to increase faster)
#2) Temp Down: Will Lower The Set Temperature Value down one point (Hold to decrease faster)
#3) Low Temp:  Timer In 5 Seconds to Lower Current Temperature to 550* and then raise back to Set Temperature once 550* has been reach. (Option to Change Temperature in Settings Menu.)
#4) Clean Mode: Time in 10 Seconds will change Set Temperature to 850* and have a timer that will run for 20 Minutes. Once 20 Minutes has been reached, change Set Temperature to original Set Temperature.
#5) Set: When Temp Up or Temp Down is used to change Variable of SET TEMPERATURE, Set will be pushed to save and finalize the temperature change.


#Schedule
#Schedule will Display:
#1) Days of the Week and Time Blocks that are selected for Heating Element to be on and Holding Set Temperatures. (3 Time Blocks are able to be selected during each day.
#2) TOP RIGHT: Will Display if Heating Element Is Currently On or Off and Current Temperature.
# Schedule Buttons:
#1) Save/Update: Selected to Finalze changes made to schedule once made.
#2) Reset: Clear Schedule of previous Time Blocks.

#Settings:
# Settings will Display Options For:
#1) Temperature:
#	1)  Set Temperature: Current Temperature that is Defaulted when Heating Element 		Is activated
#	2)  Low Temperature: Current Temperature that is Defaulted when Low Temp
#		Button is activated from Home screen or from Application or Web Access.
#	3) Heat/Clean Temperature: Current Temperature that is Defaulted when Clean
#		Button is activated from Home Screen of from Application or Web Access.
#2) Temperature Timers:
#	1) Temp Variance: Allows Option for Adjustable Timer to Turn Off Heating Element when Temperature does not exceed selected degree for certain amount of time
#Options:  1) Temp Variance – On/Off  
#	      2)Time – Set Timer for Task to run in 
#	      3)Degree– Set Between 3 and 10 Degrees for when exceeded timer is reset.
#	2) Low Temp: On/Off – Temperature Set- Set Temperature to reach before heat 	activated
#	3)Clean Temp: On/Off – Temp – Set Temperature for Clean Task to reach when 	activated.

#3)WIFI/Bluetooth
#	1) Network Settings: Shows Current Settings and Options to Add Private 	Networks or Others Accessed at a later time.
#	2) Bluetooth: On/Off : Option to Auto Connect To devices to control from near 	distance.
# Settings Buttons:
#	1) Save/Update: Selected to finalize changes made to Setting's Menu.
#	2) Reset: Resets All Settings To Factory Default Settings.



#Current Information is only accessible via web and current temperature is displaced from I2C Display connected.
#Elimination of Pump Button will be necessary as only one Heating element and device is being controlled by device. Possible options for more heating elements in the future.

#Will send more resources if needed.

#iSPRESSO:  Coffee Evolved

## Computer controlled, wifi enabled Espresso machine based on Raspberry Pi, written in Python


![iSPRESSO](https://bitbucket.org/veggiebenz/pyspresso/raw/master/img/ispresso2.png "iSPRESSO closeup")


##iSPRESSO features:

* Programmable [PID Controller](https://en.wikipedia.org/wiki/PID_controller "PID Controller") for precise boiler temperature control
* Programmable Pre-soak time, wait time, and brew time
* Controllable from web browser, iPad, iPhone (Android coming soon) on Wifi network
* Schedule allows programmable on / off timing for each day of the week
* LCD readout for system status, toggle buttons for operation


![iSPRESSO](https://bitbucket.org/veggiebenz/pyspresso/raw/master/img/ispresso1.png "iSPRESSO tall")


#Parts used:

* Rancilio Silvia Espresso machine
* Raspberry Pi Revision B, with power supply
* Adafruit Pi Cobbler Breakout kit
* small breadboard
* wifi dongle
* 2x Solid State Relay (SSR)
* 2x16 LCD with i2c backpack 
* 2x LED toggle buttons
* 1-wire temperature sensor
* 4" diameter hose clamp
* heat transfer grease
* some wires, solder, connectors, etc



#Tools used:

* Soldering Iron
* Assorted Screwdrivers
* Needlenose pliers
* Wire strippers
* Dremel
* Power drill
* 16mm Hole Saw
* Rivet Gun
* nibbler


#Screenshots:

* iSPRESSO Home Page


![iSPRESSO](https://bitbucket.org/veggiebenz/pyspresso/raw/master/img/ispresso_home.png "iSPRESSO home page")



* iSPRESSO Scheduler


![iSPRESSO](https://bitbucket.org/veggiebenz/pyspresso/raw/master/img/ispresso_schedule.png "iSPRESSO scheduler")
