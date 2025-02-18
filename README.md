# Example Project - Live Heart Rate Dashboard

This example project provides a live heart rate monitoring dashboard using Bluetooth Low Energy (BLE) technology to connect to a heart rate monitor. The heart rate data is displayed in real-time and visualized through an interactive chart. Additionally, the battery level of the heart rate monitor is also displayed.

## Features

- **Real-time Heart Rate Data**: Displays live heart rate in beats per minute (BPM).
- **Battery Level**: Displays the current battery level of the heart rate monitor.
- **Interactive Chart**: A line chart showing heart rate over time, updated in real-time.
- **BLE Connectivity**: Uses Bluetooth Low Energy to connect to compatible heart rate monitors.

## Requirements

- A web browser that supports the Web Bluetooth API (e.g., Google Chrome).
- A compatible heart rate monitor that supports Bluetooth Low Energy (BLE) and the Heart Rate service.
  
## How to Use

1. **Connect to the Heart Rate Monitor**: 
   - Click the **Connect** button on the webpage.
   - The page will scan for available BLE devices that support the Heart Rate service.
   
2. **Monitor Heart Rate**: 
   - Once connected, the heart rate monitor will start sending heart rate data to the dashboard.
   - Your heart rate will be displayed in beats per minute (BPM) in the format: `Heart Rate: XX BPM`.

3. **View Battery Level**: 
   - The battery level of the connected heart rate monitor is displayed in percentage next to the heart rate.

4. **View Real-time Graph**:
   - A line chart will display your heart rate over time, updating dynamically as new data is received.

## How It Works

- **Bluetooth Connectivity**: The app connects to a BLE heart rate monitor using the Web Bluetooth API, which allows web pages to communicate with Bluetooth devices.
- **Heart Rate Measurement**: The heart rate monitor sends heart rate data, which is processed and displayed on the page.
- **Battery Service**: The battery level of the device is retrieved using the `battery_service` and shown in percentage.
- **Charting**: The heart rate data is plotted on a line chart using the Chart.js library.

## Technologies Used

- **Web Bluetooth API**: For connecting to and interacting with BLE devices.
- **Chart.js**: For visualizing the heart rate data in real-time.
- **HTML5, CSS, and JavaScript**: For the structure, styling, and interactivity of the webpage.

## Project Structure

- **index.html**: The main HTML file containing the dashboard layout, JavaScript code for Bluetooth interaction, and heart rate charting.
- **Chart.js**: Used to create an interactive, real-time chart for displaying heart rate data.

## Demo

To test the application, you can use a compatible heart rate monitor with Bluetooth Low Energy support. Simply open the `index.html` file in a supported browser and click **Connect** to start monitoring your heart rate in real-time.

## Contributions

Feel free to fork this project, submit issues, and contribute improvements. Contributions and suggestions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
