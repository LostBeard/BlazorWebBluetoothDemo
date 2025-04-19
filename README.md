# BlazorWebBluetoothDemo

Demonstrates the Web Bluetooth API in a Blazor WebAssembly application using [SpawnDev.BlazorJS](https://github.com/LostBeard/SpawnDev.BlazorJS).

Code is based on a Javascript version:  
[ESP32 Web Bluetooth (BLE): Getting Started Guide](https://randomnerdtutorials.com/esp32-web-bluetooth/)

# Freenove ESP32-S3-WROOM-1 Cam Board


# ESP32 Code
The folder `ESP32BLEApp` contains a [PlatformIO VSCode](https://platformio.org/install/ide?install=vscode) project for an ESP32-S3-WROOM microcontroller that will act as a BLE server. The ESP32 app is written using the C programming language.
The ESP32 will advertise a service with a characteristic that can be read and written to by the Blazor WebAssembly application. No wiring is required for this demo. An onboard LED can be toggle on and off using the Blazor WASM web app and data can be retrieved automatically when it changes.
I specifically tested using the [Freenove Basic Starter Kit for ESP32-S3-WROOM CAM](https://store.freenove.com/products/fnk0084).

The Blazor WASM app is written in C# and uses the [Web Bluetooth API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API) to access services on the ESP32.

Feel free to open an issue if you have any questions or problems. Setting up the development environemnt and getting the ESP32 to work as expected (especially the drivers) can be tricky. I will try to help if I can. 🖖

