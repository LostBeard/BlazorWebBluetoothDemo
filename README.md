# Blazor Web Bluetooth Demo 🚀

Welcome to the **Blazor Web Bluetooth Demo**! This project showcases how to use the Blazor WebAssembly (WASM) framework with the Web Bluetooth API to communicate with an ESP32-S3-WROOM microcontroller board. Whether you're a developer looking to explore Bluetooth technology or a hobbyist interested in microcontrollers, this demo provides a solid foundation for your projects.

[![Blazor Web Bluetooth](https://img.shields.io/badge/Blazor%20Web%20Bluetooth-Demo-blue.svg)](https://github.com/LostBeard/BlazorWebBluetoothDemo)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The **Blazor Web Bluetooth Demo** demonstrates communication between a Blazor WASM web application and an ESP32-S3 using Bluetooth Low Enery commincation via the Web Bluetooth API. With [SpawnDev.BlazorJS](https://github.com/LostBeard/SpawnDev.BlazorJS), you can create Blazor WASM web pages that interact with various Bluetooth Low Energy (BLE) devices. This project aims to demonstrate the integration of Bluetooth technology into web applications, making it accessible for developers of all skill levels.

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
├── sdkconfig.freenove_esp32_s3_wroom   # PlatformIO test runner files
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

We welcome contributions to enhance the **Blazor Web Bluetooth Demo**. If you have suggestions or improvements, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/YourFeature
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please reach out to the repository owner:

- **Todd Tanner**  
- [GitHub Profile](https://github.com/LostBeard)  
- [Email](mailto:todd@spawndev.com)

## Conclusion

Thank you for checking out the **Blazor Web Bluetooth Demo**! We hope this project inspires you to explore the possibilities of web applications and Bluetooth technology. Happy coding!
