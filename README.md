# Gyroscope

This project demonstrates how to interact with the Gyroscope sensor on supported devices using JavaScript. It simulates the movement of a ball on the screen based on gyroscope sensor data (for mobile devices) or simulated data (for desktop browsers or devices without a gyroscope).

## Features
- **Real-time gyroscope sensor reading**: Uses the device's gyroscope to move a ball on the screen.
- **Debug mode**: Simulates gyroscope behavior on devices without sensors for easy testing on desktops.
- **Permissions handling**: Requests permissions to access gyroscope data on devices that require it.


## Getting Started

### Prerequisites

- A modern web browser (Google Chrome, Safari, or any browser that supports the Gyroscope API).
- Mobile device (such as Android or iOS) to test the gyroscope functionality.
- For testing on desktops or devices without gyroscopes, **debug mode** can be enabled.

### Setup

1. Clone the repository or download the HTML file.
2. Open the `index.html` file in your web browser.
3. Move your mobile device to see the ball moving on the screen based on gyroscope data.

### Debug Mode (for desktop browsers)

If you are testing on a desktop or laptop that doesn't have a gyroscope, you can enable **debug mode**. In this mode, simulated data will move the ball:

1. Open the `index.html` file.
2. In the `<script>` section, set `debugMode` to `true`:
   
    ```javascript
    const debugMode = true;
    ```
4. Refresh the page to see the simulated gyroscope motion.

### Permissions

Some mobile browsers might require permission to access the gyroscope. If your browser prompts for permission, allow access for the ball animation to work correctly.

### Compatibility

- Mobile Devices: The gyroscope functionality works on mobile devices such as iPhones and Android devices that support the Gyroscope API.
- Desktop Browsers: For devices that do not have a gyroscope, the ball can be moved using **debug mode**. The simulation provides a smooth approximation of actual gyroscope behavior.

## Code Explanation

- **Gyroscope API**: The code uses the `Gyroscope` API to read sensor data and update the position and rotation of the ball on the screen.
- **CSS Animation**: The ball is styled using `radial-gradient` and CSS `transform` properties for smooth movement and rotation.
- **Permissions API**: For devices that require permission, the code requests access to the gyroscope sensor using the `Permissions API`.


## Acknowledgments

- Thanks to the developers who contributed to the Gyroscope API and web standards.
- This project was inspired by the growing trend of incorporating real-time sensor data in web applications.
