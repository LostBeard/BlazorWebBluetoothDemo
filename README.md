# Blazor Web Bluetooth Demo 🚀

Welcome to the **Blazor Web Bluetooth Demo**! This project showcases how to use the Blazor WebAssembly (WASM) framework with the Web Bluetooth API to communicate with an ESP32-S3-WROOM microcontroller board. Whether you're a developer looking to explore Bluetooth technology or a hobbyist interested in microcontrollers, this demo provides a solid foundation for your projects.

![Blazor Web Bluetooth](https://img.shields.io/badge/Blazor%20Web%20Bluetooth-Demo-blue.svg)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Introduction

The **Blazor Web Bluetooth Demo** enables seamless communication between web applications and Bluetooth devices. By leveraging the capabilities of the ESP32-S3-WROOM microcontroller, you can create applications that interact with various Bluetooth Low Energy (BLE) devices. This project aims to simplify the integration of Bluetooth technology into web applications, making it accessible for developers of all skill levels.

## Features

- **Web Bluetooth API Integration**: Directly connect and communicate with BLE devices.
- **ESP32-S3-WROOM Support**: Utilize the powerful features of the ESP32-S3 microcontroller.
- **Blazor WebAssembly**: Build interactive web applications using C# and .NET.
- **Real-time Data Exchange**: Send and receive data between the web app and Bluetooth devices.
- **User-friendly Interface**: Simple and intuitive UI for easy interaction.

## Getting Started

To get started with the **Blazor Web Bluetooth Demo**, follow these steps:

1. **Clone the Repository**: Use the following command to clone the repository:
   ```bash
   git clone https://github.com/LostBeard/BlazorWebBluetoothDemo.git
   ```
   
2. **Navigate to the Project Directory**:
   ```bash
   cd BlazorWebBluetoothDemo
   ```

3. **Install Dependencies**: Ensure you have the necessary dependencies installed. You can use the following command:
   ```bash
   dotnet restore
   ```

4. **Run the Application**: Start the application with:
   ```bash
   dotnet run
   ```

5. **Open Your Browser**: Navigate to `http://localhost:5000` to view the application.

## Usage

Once the application is running, you can interact with Bluetooth devices. Here’s how:

1. **Connect to a Device**: Click the "Connect" button to scan for available Bluetooth devices.
2. **Select a Device**: Choose a device from the list and establish a connection.
3. **Send Data**: Use the provided interface to send data to the connected device.
4. **Receive Data**: Monitor incoming data from the device in real-time.

## Project Structure

The project is organized as follows:

```
BlazorWebBluetoothDemo/
├── wwwroot/                # Static files
│   ├── css/                # Stylesheets
│   ├── js/                 # JavaScript files
│   └── index.html          # Main HTML file
├── Pages/                  # Blazor pages
│   ├── Index.razor         # Main page
│   └── ...                 # Other pages
├── Shared/                 # Shared components
│   └── ...                 # Shared components
├── BlazorWebBluetoothDemo.csproj # Project file
└── Program.cs              # Entry point
```

## Technologies Used

This project uses the following technologies:

- **Blazor WebAssembly**: A framework for building interactive web applications using C#.
- **Web Bluetooth API**: A JavaScript API that allows web applications to communicate with Bluetooth devices.
- **ESP32-S3-WROOM**: A powerful microcontroller with built-in Bluetooth capabilities.
- **C#**: The primary programming language used in this project.
- **HTML/CSS**: For building the user interface.

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

## Releases

You can download the latest releases of the **Blazor Web Bluetooth Demo** from the [Releases section](https://github.com/LostBeard/BlazorWebBluetoothDemo/releases). Here, you will find compiled versions and updates. 

Feel free to check the [Releases section](https://github.com/LostBeard/BlazorWebBluetoothDemo/releases) for any updates or new features.

## Conclusion

Thank you for checking out the **Blazor Web Bluetooth Demo**! We hope this project inspires you to explore the possibilities of web applications and Bluetooth technology. Happy coding!
