This project is a placeholder reminding me what has to be done to make an esp32 build, compile, and debug in vscode.

Install the Arduino and 'auto scroll' extensions (auto scroll is useful for build and Serial output).  RTFM for 'auto scroll'
and make sure to enable it on the terminal window.

This requires openocd as well as the Arduino IDE which must be installed as part of the esp-idf tool suite.

Make sure to update your project's 3 json files in your .vscode directory to look like the ones here.

Right now the paths in the .vscode json are hardcoded for my osx configuration.  I will do better later.  Search for the string 'path' in the json files and update to point to where the esp-idf tools and the Arduino IDE tools live.  The 'output' json clause in aduino.json quiets the complaint about 'slow builds', and avoids a complete object tree being built (and discarded) for each run.

This was tested with an esp32-wroom and a ESP-prog JTAG dongle.  Both devices were plugged into usb to my MBP.  The json configuration references those ports explicitly.

Oddities:

Any Arduino IDE operation pops up the Arduino splash screen.  Google searches show the problem was fixed and is broken again.  I will have to tough it out in the meantime.  Also, debugging causes the Arduino 'validate' build to occur, and I can't figure out how to disable it.
