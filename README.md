# Blazor Web Bluetooth Demo 🚀

Welcome to the **Blazor Web Bluetooth Demo**! This project showcases how to use the Blazor WebAssembly (WASM) framework with the Web Bluetooth API to communicate with an ESP32-S3-WROOM microcontroller board. Whether you're a developer looking to explore Bluetooth technology or a hobbyist interested in microcontrollers, this demo provides a solid foundation for your projects.

[![Blazor Web Bluetooth](https://img.shields.io/badge/Blazor%20Web%20Bluetooth-Demo-blue.svg)](https://github.com/LostBeard/BlazorWebBluetoothDemo)

## Table of Contents

- [Introduction](#introduction)
- [References](#references)
- [Live Demo](#live-demo)
- [Getting Started](#getting-started)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

- The **Blazor Web Bluetooth Demo** demonstrates communication between a Blazor WASM web application and an ESP32-S3 using Bluetooth Low Energy communication via the [Web Bluetooth API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API). 
- The `ESP32BLEApp` folder contains a [VSCode with PlatformIO](https://platformio.org/install/ide?install=vscode) project that runs on the ESP32-S3-WROOM board and hosts a BLE GATT Service that provides access to data and control over GPIO pins. 
- The `BlazorWebBluetoothDemo` folder contains a Blazor WebAssembly project that uses the Web Bluetooth API to communicate with the GATT Service running on the ESP32 wirelessly.
- [SpawnDev.BlazorJS](https://github.com/LostBeard/SpawnDev.BlazorJS) is used to access the [Web Bluetooth API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API).

## References

- [Web Bluetooth API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API) - developer.mozilla.org
- [ESP32-S3-WROOM](https://store.freenove.com/products/fnk0085) - store.freenove.com
- [PlatformIO](https://platformio.org/) - platformio.org
- [Blazor WebAssembly](https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor) - dotnet.microsoft.com
- [Introduction to Bluetooth Low Energy](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gatt) - learn.adafruit.com
- [GATT Services](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gatt#services-640991) - learn.adafruit.com
- [GATT Service Characteristics](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gatt) - learn.adafruit.com

## Live Demo 

- Run the `ESP32BLEApp` app on your ESP32-S3-WROOM board
- Run the [Live Demo](https://lostbeard.github.io/BlazorWebBluetoothDemo/)

## Getting Started

- Clone the repo.
- Upload and run the `ESP32BLEApp` project on your ESP32-S3-WROOM board using [PlatformIO](https://platformio.org/install/ide?install=vscode).
- The ESP32 app will run a BLE GATT Service with two [Characteristics](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gatt#characteristics-640991):
  - `LED` - used to control the onboard LED.
  - `Sensor` - used to read the current value of a fake sensor.
- Open the `BlazorWebBluetoothDemo` project in Visual Studio.
- Build and run the Blazor WebAssembly project to start the demo in a new browser window.
- Click `Connect to BLE Device` to see a list of available Bluetooth devices. 
- Select `ESP32` to `Pair` your ESP32-S3-WROOM board to the Blazor web app.
- The Blazor app will:
  - Request a specific GATT Service running on the ESP32.
  - Get a specific GATT Service Characteristic from that GATT Service.
  - Read the GATT Service Characteristic's current value.
  - Subscribe to value change events for that GATT Service Characteristic and update the value shown.
- Click the `ON` and `OFF` buttons to control the ESP32's onboard LED accessed via another GATT Service Characteristic.

## Features

- **Web Bluetooth API Integration**: Directly connect and communicate with BLE devices.
- **ESP32-S3-WROOM Support**: Utilize the powerful features of the ESP32-S3 microcontroller.
- **Blazor WebAssembly**: Build interactive web applications using C# and .NET.
- **Real-time Data Exchange**: Send and receive data between the web app and Bluetooth devices.

## ESP32-S3-WROOM
This project uses the ESP32-S3-WROOM microcontroller board, which is a powerful and versatile platform for building IoT applications. The ESP32-S3 features built-in Bluetooth Low Energy (BLE) capabilities, making it an ideal choice for this demo.  

![ESP32-S3-WROOM Board](https://raw.githubusercontent.com/LostBeard/BlazorWebBluetoothDemo/master/BlazorWebBluetoothDemo/wwwroot/ESP32-S3-WROOM.jpg)

## Project Structure

The project is organized as follows:

```
ESP32BLEApp/                            # ESP32 PlatformIO project
├── include/                            # Project header files
├── lib/                                # Project library files
├── src/                                # Project
│   ├── CMakeLists.txt                  # CMake list
│   ├── main.cpp                        # Entry point
├── test/                               # PlatformIO test runner files
├── sdkconfig.freenove_esp32_s3_wroom   # ESP32-S3-WROOM configuration file
└── platformio.ini                      # PlatformIO confiuration file
BlazorWebBluetoothDemo/                 # Blazor WebAsembly project
├── wwwroot/                            # Static files
│   ├── css/                            # Stylesheets
│   ├── js/                             # JavaScript files
│   └── index.html                      # Main HTML file
├── Pages/                              # Blazor pages
│   ├── Index.razor                     # Main page
│   └── ...                             # Other pages
├── Shared/                             # Shared components
│   └── ...                             # Shared components
├── BlazorWebBluetoothDemo.csproj       # Project file
└── Program.cs                          # Entry point
```

## Technologies Used

This project uses the following technologies:

- **Blazor WebAssembly**: A framework for building interactive web applications using C#.
- **C#**: The primary programming language used for the Blazor WASM project.
- **HTML/CSS**: For building the user interface.
- **Web Bluetooth API**: A JavaScript API that allows web applications to communicate with Bluetooth devices.
- **[PlatformIO](https://platformio.org/)**: A framework for building interactive web applications using C#.
- **C/C++**: The primary programming language used for the ESP32-S3 project.
- **[ESP32-S3-WROOM](https://store.freenove.com/products/fnk0085)**: A powerful microcontroller with built-in Bluetooth capabilities.

## Contributing

We welcome contributions to enhance the **Blazor Web Bluetooth Demo**. If you have suggestions or improvements, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

## Contact

For questions or feedback, please reach out to the repository owner:

- **Todd Tanner**  
- [GitHub Profile](https://github.com/LostBeard)  
- [Email](mailto:todd@spawndev.com)

## Conclusion

Thank you for checking out the **Blazor Web Bluetooth Demo**! We hope this project inspires you to explore the possibilities of web applications and Bluetooth technology. Happy coding!
