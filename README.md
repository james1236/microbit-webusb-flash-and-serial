# micro:bit WebUSB Flash and Serial
A minimal tool for flashing a micro:bit v2 over WebUSB and communicating using Serial.

# Usage
Run `make`, or manually run `python3 -m http.server 8080`

# Compatibility
| Device | Notes |
|---|---|
|micro:bit v2| Works, but fails with large hex files |
|micro:bit v1| Unknown |

# Dependencies
The following required files have been put in the repository:
* [dap.umd.js](https://github.com/ARMmbed/dapjs) (DAP.js is a JavaScript interface to CMSIS-DAP, enabling access to Arm Microcontrollers using Node.js or in the browser using WebUSB)
* [partial-flashing.js](https://github.com/bbcmicrobit/PythonEditor/blob/master/js/partial-flashing.js) (Taken from [bbcmicrobit/PythonEditor](https://github.com/bbcmicrobit/PythonEditor), which is an old version of a micropython programming tool for micro:bit. It was the only open-source WebUSB flasher I could find)