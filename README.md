# NNOSTime

NNOSTime is a lightweight, visually appealing web page that displays the current date and time with a futuristic design. With a gradient background, and a dynamic digital clock effect, this project provides a simple yet eye-catching way to show time.

## Features

- **Dynamic Time Display:**  
  Uses JavaScript's `Intl.DateTimeFormat` API to format and display the current time. The time updates every second for real-time accuracy.

- **Customizable Time Zone:**  
  The current implementation displays time in the 'America/New_York' time zone. You can change the `timeZone` property in the script to display a different region's time.

- **Futuristic Aesthetic:**  
  Incorporates a modern gradient background and the Orbitron font from Google Fonts to give the page a sleek, futuristic look.

- **Minimalistic Design:**  
  The design hides the default scrollbar and cursor for a cleaner user experience.

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.) that supports HTML5, CSS3, and JavaScript ES6 features.

### Installation

1. **Clone the Repository:**  
   Clone or download the source code to your local machine.
   ```bash
   git clone https://github.com/Natuworkguy/NNOSTime.git
   ```

2. **Navigate to the Project Directory:**  
   ```bash
   cd NNOSTime
   ```

3. **Open the Application:**  
   Open the `index.html` file in your preferred web browser.

## Code Overview

- **HTML Structure:**  
  The HTML file contains the basic structure, including a `<head>` with metadata, a `<style>` block for CSS, and a `<body>` that includes a heading and an element (`<b id="currentTime">`) to display the current time.

- **CSS Styling:**  
  Inline CSS is used to apply a gradient background, customize fonts, hide the scrollbar, and style the time display element with a text-shadow effect.

- **JavaScript Functionality:**  
  A script at the bottom of the HTML file:
  - Retrieves the current date and time.
  - Formats the time using `Intl.DateTimeFormat` with options for the 'America/New_York' time zone, 12-hour formatting, and specific display options for year, month, day, hour, minute, and second.
  - Updates the time every second using `setInterval`.

## Customization

- **Change the Time Zone:**  
  To display the time for a different time zone, update the `timeZone` property in the JavaScript options:
  ```javascript
  const options = {
    timeZone: 'Your/Preferred_TimeZone',
    year: 'numeric',
    month: 'short',
    day: 'numeric',
    hour: '2-digit',
    minute: '2-digit',
    second: '2-digit',
    hour12: true,
  };
  ```

- **Adjust the Appearance:**  
  Modify the CSS in the `<style>` block to change colors, fonts, or layout according to your design preferences.

- **Time Format:**  
  You can alter the formatting options in the `options` object to display the date and time in your preferred format.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgements

- The JavaScript community for the powerful and easy-to-use `Intl.DateTimeFormat` API.
