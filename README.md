# World Clock Test Project

A lightweight, single-file web application that displays the current time across multiple time zones. **Note:** This project was developed as a test project to experiment with time zone handling using native browser APIs.

[Live Demo](https://shashankpoojari.github.io/World-Clock-Test-Project/)

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [Customization](#customization)
- [License](#license)

---

## Overview

The **World Clock Test Project** is a single HTML file that dynamically displays clocks for every supported time zone on your browser. Using JavaScript and CSS, the project retrieves time zone data via the `Intl.supportedValuesOf('timeZone')` method and calculates the time difference relative to the user’s local time. The interface automatically updates every second, and user preferences (like the 12‑hour/24‑hour format) are saved using localStorage.

**This is a test project** intended for experimental demonstration purposes and to explore browser-based time zone functionalities.

---

## Features

- **Dynamic Updates:** Clocks refresh every second to show current times.
- **Time Zone Detection:** Automatically detects and highlights your local time zone.
- **Search Functionality:** Quickly filter time zones using the search box.
- **Time Format Toggle:** Easily switch between 12‑hour and 24‑hour formats with user preferences saved across sessions.
- **Responsive Design:** Optimized for desktops, tablets, and mobile devices.
- **Visual Cues:** Color-coded labels indicate different parts of the day based on the current time.

---

## Demo

View the live demo here:  
[https://shashankpoojari.github.io/World-Clock-Test-Project/](https://shashankpoojari.github.io/World-Clock-Test-Project/)

---

## Usage

- **Time Format:** Use the dropdown at the top to switch between 12‑hour and 24‑hour formats.
- **Search:** Begin typing in the search box to filter time zones by name.
- **Scroll-to-Top:** A scroll-to-top button appears when you scroll down; click it to quickly return to the top of the page.

The clocks continuously update to reflect the current time and date in each time zone along with a calculated time difference relative to your local time zone.

---

## Code Structure

- **index.html:** Contains the entire application’s HTML, embedded CSS, and JavaScript.
  - **CSS:** Defined in a `<style>` block within the `<head>` section. It uses CSS variables for easy customization of the color scheme and layout.
  - **JavaScript:** Included in a `<script>` block at the end of the file. The main class (`WorldClock`) handles loading time zones, updating clocks every second, filtering results based on user input, and managing the time format toggle.
  
All logic is self-contained in this single file for simplicity and ease of testing.

---

## Customization

- **Styling:** You can adjust the color scheme and layout by editing the CSS variables in the `:root` selector.
- **Time Zones:** The project uses the browser’s native `Intl.supportedValuesOf('timeZone')` to retrieve time zone data. To modify which time zones are displayed or change the sorting criteria, adjust the relevant methods in the JavaScript section.
- **Time Format:** The dropdown allows switching between 12‑hour and 24‑hour formats. User selections are stored in localStorage, so you can remove or modify that logic if needed.

---

## License

This project is released under the **CC0-1.0 license**, dedicating it to the public domain. You are free to use, modify, and distribute it without any restrictions.  
For complete details, see the [LICENSE](LICENSE) file in the repository.
