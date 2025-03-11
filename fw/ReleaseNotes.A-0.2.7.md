# PGI Filter Analyzer Firmware

## ver. A-0.2.7

**New Features:**
* Barcode capture confirmation page - will prompt user if it is accept or retake image
    * If image is accepted, spinner will be brought up as barcode is decoded
    * If barcode is successfully decoded, a bounding box will be drawn around barcode with decoded text
    * If barcode is NOT successfully decoded, image will be crossed and relevant error feedback will be displayed 
* Adds optional text field for additional test notes: right below filter age and filter type dropdowns
    * Note that this diagnostics need to be turned on in settings
* Adds pop up notification to signal upload status to user
    * Will display success message or relevant error information
* Full power off timer to help conserve battery
    * Will turn off device after 5 minutes of inactivity
    * Screen will go into standby mode after 2 minutes of inactivity 
* Ability to wake up device with touch screen and button inputs from low power mode
* Ability to wake up device from low power mode via USB plug in event 
* Low power charging screen/state - will go into this state at boot if charging or if device is powered off and charging
* Turns on backlight and brings up bootup message sooner: more immediate feedback for user

**Fixes:**
* Fixes camera settings for improved performance in low light conditions
    * Changes to RGB565 (full color) instead of monochrome stream
    * Activate autoexposure and autogain control
* Fixes hanging network timers preventing handling of power interrupts
    * Moved time set task to task outside of network timer  
* Fixes Unknown typo in diagnostics filter info page
* Fixes incorrect sample time label -> now 10 seconds instead of 6 seconds
* Fixes keypad navigation issue in settings page -> no longer require double presses for beep and diagnostics
