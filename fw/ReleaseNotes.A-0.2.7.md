# PGI Filter Analyzer Firmware

## ver. A-0.2.7

**New Features:**
* Barcode capture confirmation page - will prompt user to accept or retake image
    * If image is accepted, loading wheel will be spawned as barcode is decoded
* VIN decoding feedback page - spawned after accepting image capture
    * If barcode is successfully decoded, a bounding box will be drawn around barcode with decoded text
    * If barcode is NOT successfully decoded, image will be crossed and relevant error feedback will be displayed 
* Adds optional text field for additional test notes: right below filter age and filter type dropdowns
    * Note that diagnostics input need to be turned on in the settings page
* Adds color camera stream and improved settings for low light conditions
    * Activate autoexposure and autogain control
    * Changes to RGB565 (full color) instead of monochrome stream for better vis
* Adds pop up notification to signal upload status to user
    * Will display success message or relevant error information in pop up window
    * Window is spawned in the background and will dissapear after 2 seconds (duration can be changed in future FW if necessary)
* Full power off timer to help conserve battery
    * Will turn off device after 30 minutes of inactivity
    * Screen will go into standby mode after 2 minutes of inactivity 
* Ability to wake up device with touch screen and button inputs from low power mode
* Ability to wake up device from low power mode via USB plug in event 
* Low power charging screen/state - will go into this state at boot if charging or if device is powered off and charging
* Turns on backlight and brings up bootup message sooner: more immediate feedback for user

**Fixes:**
* Fixes hanging network timers preventing handling of power interrupts
    * Moved time set task to task outside of network timer  
* Fixes Unknown typo in diagnostics filter info page
* Fixes incorrect sample time label -> now 10 seconds instead of 6 seconds
* Fixes keypad navigation issue in settings page -> no longer require double presses for beep and diagnostics
