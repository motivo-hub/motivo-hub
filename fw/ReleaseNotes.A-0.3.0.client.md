# PGI PureFlow ViAQ Analyzer Firmware

## ver. A-0.3.0

**New Features:**
* After a filter replacement procedure, the Results screen will now show the filtration percentage of both the Old and New filters
* After a Measurement Re-run, the Results screen will now show the filtration percentage of both the Old and New measurments
* On a normal Mesurement, the User is no longer requested to take an Ambient Measurement if one has been taken in the last hour
* On a Measurement Re-run, the User is now requested to take a new Ambient Measurement 
* In the filter type dropdown menu, "Unknown" type is now supported

**Fixes:**
* When USB is disconnected while in Standby, system now powers down
* Wake up from Standby now requires a 2+ seconds Power Button press
* The security of the Keys for Cloud data upload has now been enhanced 


## ver. A-0.2.7

**New Features:**
* VIN Barcode Image
  * After image capture, an accept/retake dialog is now shown 
  * During image decoding, a "loading" spinner is now displayed
  * After image decoding, the decoded characters are now displayed
  * On image decode failure, the image is crossed out in red
* In Diagnostics Mode, before Cabin Air Measurement, a text box is provided for entry of extra notes
* Camera settings are now improved for difficult lighting conditions
* A pop-up notification in the background now signals data Upload status
* System will now power down after 30 minutes of Standby (Screen OFF) 
* System can now be woken up from Standby (Screen OFF) by input from Touch Screen or Buttons, or USB plug-in
* If charging ad the System powers down (from Power Button or Standby inactivity), the Charging Screen is now displayed 

**Fixes:**
* System now correctly reponds to USB power changes
* System will now no longer crash if too many WiFi Access Points are detected
* The Beep and Diagnostics settings buttons no longer require a double click


## ver. A-0.1.7

**New Features:**
* System will now go to Standby (Screen OFF) after 2 minutes of inactivity on Touch Screen or Buttons 
* System will now power down after 5 minutes of Standby
* System bootup speed has been improved

**Fixes:**
* "Unknown" filter type in diagnostics filter info page, is now correctly spelled
* Measurement test duration is now correctly shown as 10 seconds (instead of 6 seconds)


## ver. A-0.0.7

**New Features:**
* System wake up on USB-C power, or 2s Power Button press
* PGI Welcome screen
* Status bar: battery charging icon and percentage SOC
* Status bar: Wifi and Time of Day
* Screen OFF with short Power Button press
* System powers off to long shelf life mode, with 3s Power Button press
* Settings page shows version number and MAC ID
* List of available Wifi SSIds is shown
* Wifi SSID selectio and password entry supported
* Manual Time Zone entry supported
* Audible beeps on button presses (disabled in Settings)
* Camera for VIN scanning supported (barcode decoding in Cloud)
* 6s Ambient particle measurement
* Filter type/age entry supported in Diagnostics mode (enabled in Settings)
* 6s Cabin Air Test
* Estimated Filter age color graphic
* Particle count details available in "Details" page
* Test re-run UI flow provided
* Filter replacement UI flow provided  
* Camera images & particle data uploaded to Cloud

**Fixes:**
* N/A - first release