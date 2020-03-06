This project is a placeholder reminding me what has to be done to make an esp32 build, compile, and debug in vscode.

Install the Arduino and 'auto scroll' extensions (auto scroll is useful for build and Serial output).  RTFM for 'auto scroll'
and make sure to enable it on the terminal window.

Right now the paths in the .vscode json are hardcoded for my osx configuration.  I will do better later.

This was tested with an esp32-wroom and a ESP-prog JTAG dongle.  Both devices were plugged into usb to my MBP.  The json configuration
references those ports explicitly.

This requires openocd as well as the Arduino IDE which must be installed as part of the esp-idf tool suite.
