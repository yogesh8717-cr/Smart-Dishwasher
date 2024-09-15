# Smart Dishwasher Dashboard

A modern, responsive web dashboard interface for controlling and monitoring a smart dishwasher. The dashboard includes features such as selecting wash cycles, viewing real-time data during a cycle, accessing cycle history, and adjusting various settings.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Cycles Tab](#cycles-tab)
  - [Real-Time Data Tab](#real-time-data-tab)
  - [Cycle History Tab](#cycle-history-tab)
  - [Settings Tab](#settings-tab)
- [Code Structure](#code-structure)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Demo

![Smart Dishwasher Dashboard Screenshot](screenshot.png)

*Note: Include a screenshot of the dashboard here.*

## Features

- **Cycle Selection**: Choose from various wash cycles like Normal, Eco, Intensive, and Quick.
- **Real-Time Monitoring**: View live updates on cycle progress, water usage, energy consumption, and estimated time remaining.
- **Cycle History**: Access a comprehensive history of past cycles with details like date, cycle type, duration, water used, and energy consumed. View total and average usage statistics.
- **Settings**: Configure connectivity options, display settings, and system preferences. Includes features like Wi-Fi setup, language selection, brightness adjustment, child lock, software updates, and factory reset.
- **Responsive Design**: Optimized for various devices, including desktops, tablets, and mobile phones.
- **Interactive UI**: Modern design with smooth transitions, hover effects, and intuitive controls.

## Technologies Used

- **HTML5**: Semantic markup and structure.
- **CSS3**: Styling and responsive design using flexbox and media queries.
- **JavaScript**: Dynamic content updates, event handling, and simulations.

## Getting Started

### Prerequisites

- A modern web browser (e.g., Chrome, Firefox, Safari, Edge).
- Optional: A local web server for hosting the dashboard (e.g., Live Server extension for VSCode).

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/smart-dishwasher-dashboard.git
   ```

   Or download the ZIP file and extract it.

2. **Navigate to the Project Directory**

   ```bash
   cd smart-dishwasher-dashboard
   ```

3. **Open the Dashboard**

   - Simply open the `index.html` file in your preferred web browser.
   - Alternatively, you can serve it using a local web server for a more accurate experience.

## Usage

### Cycles Tab

1. **Select a Cycle**

   - Click on one of the cycle cards to select a wash cycle.
   - The available cycles are:
     - **Normal**: Standard cleaning for everyday dishes.
     - **Eco**: Energy-efficient cycle that saves water and electricity.
     - **Intensive**: High-power cycle for heavily soiled dishes.
     - **Quick**: Fast cycle for lightly soiled dishes.

2. **Start the Cycle**

   - After selecting a cycle, click the **Start Cycle** button.
   - The button will change to "Cycle Running..." and will be disabled during the cycle.

### Real-Time Data Tab

- **Monitoring Progress**

  - Automatically redirected here after starting a cycle.
  - View the progress circle indicating the percentage completion.
  - Real-time updates on:
    - **Water Usage**: Displays the amount of water used in liters.
    - **Energy Consumption**: Shows the energy consumed in kilowatt-hours (kWh).
    - **Estimated Time**: Indicates the total time of the cycle in minutes.

- **Completion**

  - An alert will notify you when the cycle is completed.
  - The dashboard will reset, allowing you to start a new cycle.

### Cycle History Tab

- **Summary Statistics**

  - View total cycles run, total water used, total energy consumed, and average energy per cycle.

- **Detailed History**

  - A table listing all past cycles with details:
    - **Date**
    - **Cycle Type**
    - **Duration**
    - **Water Used**
    - **Energy Consumed**

- **Interactivity**

  - Hover over table rows to highlight them for better readability.

### Settings Tab

#### Connectivity Settings

- **Wi-Fi Configuration**

  - Enter your Wi-Fi network name (SSID) and password.

- **Notifications**

  - Toggle to enable or disable notifications.

- **Check for Updates**

  - Click the **Check for Updates** button to simulate checking for software updates.

- **Save Settings**

  - Click **Save Settings** to apply and save your connectivity preferences.

#### Display Settings

- **Language Selection**

  - Choose your preferred language from the dropdown menu.

- **Brightness Adjustment**

  - Use the slider to adjust the display brightness.

- **Child Lock**

  - Toggle to enable or disable the child lock feature.

- **Reset to Defaults**

  - Click the **Reset to Defaults** button to simulate a factory reset.
  - A confirmation dialog will appear before proceeding.

- **Save Settings**

  - Click **Save Settings** to apply and save your display preferences.

## Code Structure

- **index.html**

  - Contains the entire code for the dashboard, including HTML, CSS, and JavaScript.

- **HTML Structure**

  - The main sections are:
    - `<header>`: Contains the dashboard title.
    - `<nav>`: Navigation menu with tabs.
    - `<main>`: Main content area with tab contents.
    - `<footer>`: Footer information.

- **CSS Styles**

  - Defined within `<style>` tags in the `<head>` section.
  - Uses CSS variables for color theming and consistency.
  - Organized into sections for global styles, tabs, components, and responsive design.

- **JavaScript Code**

  - Located at the end of the `<body>` inside `<script>` tags.
  - Handles:
    - Tab navigation and content switching.
    - Cycle selection and simulation.
    - Real-time data updates.
    - Cycle history management.
    - Settings form submissions and interactions.

## Customization

- **Styling**

  - Modify CSS variables in the `:root` selector to change the color scheme.
  - Customize fonts by changing the Google Fonts import link.

- **Adding Cycles**

  - To add new wash cycles, duplicate a `.cycle-card` div in the **Cycles Tab** section.
  - Update the `data-cycle` attribute and cycle details accordingly.
  - Ensure to handle the new cycle type in the `startCycle()` function in JavaScript.

- **Extending Functionality**

  - Implement actual data storage and retrieval using localStorage or a backend service.
  - Replace alert messages with custom modal dialogs for better user experience.
  - Integrate real hardware communication for a fully functional smart dishwasher.

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork the Repository**

   Click the **Fork** button at the top right corner of the repository page.

2. **Create a Branch**

   ```bash
   git checkout -b feature/YourFeatureName
   ```

3. **Commit Your Changes**

   ```bash
   git commit -am 'Add your feature'
   ```

4. **Push to the Branch**

   ```bash
   git push origin feature/YourFeatureName
   ```

5. **Open a Pull Request**

   Navigate to your forked repository and click the **New Pull Request** button.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

- **Icons**

  - Unicode icons are used for simplicity in the settings buttons.
  - Consider using [Font Awesome](https://fontawesome.com/) or [Material Icons](https://material.io/resources/icons/) for more variety.

- **Fonts**

  - [Roboto Font](https://fonts.google.com/specimen/Roboto) by Google Fonts.

- **Inspiration**

  - The design and functionality are inspired by modern IoT device dashboards and smart home applications.
