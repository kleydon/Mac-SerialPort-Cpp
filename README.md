# Mac-SerialPort-Cpp

A serial port class for the Mac, written in C++, for interfacing microcontrollers, etc. Works over USB serial.


## Usage:

* Open serial port for a device with: `openAndConfigureSerialPort(const char* portPath, int baudRate)`
* Read data using: `readSerialData(char* bytes, size_t length)`
* Write data using: `writeSerialData(const char* bytes, size_t length)`
* Remember to flush potentially buffered data when necessary with: `flushSerialData()`
* Close serial port when done, using: `closeSerialPort(void);`
