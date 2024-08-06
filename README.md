# Sury
this is a upgrade of shark firmware designed for using on esp32 m5stick c plus 1

M5BURNER is trash , if some people can help me to publish sury in m5burner i will be grated 

TOOLS 


    TV B-Gone port (thanks to MrArm's HAKRWATCH) to shut off many infrared-controlled TVs, projectors and other devices
    AppleJuice iOS Bluetooth device pairing spam
    Bluetooth device notification spamming for SwiftPair (Windows) and Android
    WiFi Spam - Funny SSIDs, WiFi Rickrolling, and a Random mode that creates hundreds of randomly-named SSIDs per minute
    WiFi NEMO Portal - A captive portal that tries to social engineer email credentials - saves usernames and passwords to SD Card (if inserted into a supported reader)
    WiFi SSID Scanner - Display 2.4 GHz SSIDs nearby, get information about them, and even clone the SSIDs in NEMO Portal
    User-adjustable 24 Hour digital clock backed by the M5 Stick RTC so it holds relatively stable time even in deep sleep and low battery mode
    EEPROM-backed Settings for rotation, brightness, automatic dimming and NEMO Portal SSID
    Battery level and credits in settings menu
    IR_AH save and replay IR signals
    RFID copy and write RFID tags

User Interface

There are three main controls:

    Home - Stops the current process and returns you to the menu from almost anywhere in SHARK

    Next - Moves the cursor to the next menu option. In function modes, this usually stops the process and returns you to the previous menu.

    Select - Activates the currently-selected menu option, and wakes up the dimmed screen in function modes

    StickC and StickC-Plus
        Power: Long-press the power button for 6 seconds to turn off the unit
        Home: Tap the power button (closest to the USB port)
        Next: Tap the side button
        Select: Tap the M5 button on the front of the unit
        M5Button presst while Startup: no Startupsound

    Cardputer
        Home: Tap the Esc/~/` key or the Left-Arrow/, key
        Next/Prev: Tap the Down-Arrow/. key and Up-Arrow/; keys to navigate
        Select: Tap the OK/Enter key or Right-Arrow/? key
        M5Button presst AFTER switch turn on: no Startupsound

NEMO Portal

In NEMO Portal mode, NEMO activates an open WiFi Hotspot named "Nemo Free WiFi" (configurable in portal.h) with DNS, DHCP and Web servers activated.

    NEMO Portal serves a fake login page that claims to provide internet access if you log in.
    This is a social engineering attack, and will log the username and passwords entered on the page.
    From the Wifi Scan details, you can clone an existing SSID from the scan list. Exiting NEMO Portal will clear the Evil Twin SSID
    You can view captured credentials by connecting to the portal from your own device and browsing to http://172.0.0.1/creds
    You can set a custom SSID by connecting to the portal from your own device and browsing to http://172.0.0.1/ssid
    If your device supports EEPROM for settings, the custom SSID you enter will be saved as the default, even if powered off.
    If your device has an SD Card reader with a FAT filesystem formatted card inserted, the usernames and passwords will be logged to nemo-portal-creds.txt on the SD Card for you to peruse later.
    SD Card support is only enabled by default on the M5Stack Cardputer platform. It can be enabled on M5Stick devices but an SD Card reader must be built and attached to the front panel pin header.
    NEMO Portal is only for use on professional engagements with a valid scope of work, educational or demonstration purposes. Storage, sale, or use of personal information without consent is against the law. 🤓
