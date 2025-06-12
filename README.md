# EAS Encoder

This project is a web-based EAS (Emergency Alert System) Encoder. It allows you to generate and play EAS tones based on configurable parameters like event type, originator, time, and location. You can also save the generated audio as a WAV file.

## Features

* **Event Selection:** Choose from a comprehensive list of weather-related and non-weather-related EAS event types.
* **Originator Selection:** Specify the alert's originator (e.g., EAS Participant, National Weather Service).
* **Time Configuration:** Set the hour, minute, and total duration for the alert.
* **Customizable Sender ID:** Define your own sender ID for the alert.
* **Attention Tone Options:** Select between NWR (1050Hz) or EBS attention tones, with adjustable duration.
* **Encoding Options:** Include extra marks for SAGE encoders or extra spaces for NWR encoding, and a "Clip Signal" option for authenticity.
* **Custom SAME Header:** Option to input a custom SAME (Specific Area Message Encoding) header.
* **Location Management:** Add and manage FIPS codes for specific locations, with options to select by state, county, and region.
* **Audio Output:** Play generated EAS tones directly in the browser and save them as a WAV file.

---

## How to Use

1.  **Open `index.html`:** Simply open the `index.html` file in your web browser.
2.  **Select Encoder Controls:**
    * Choose the **EAS Event Type** and **Originator** from the dropdowns.
    * Set the **Hour**, **Minute**, and **Time Length** for the alert.
    * Enter a **Sender ID** in the provided input field.
    * Select the desired **Attention Tone** and its **duration**.
    * Toggle the checkboxes for **Extra Marks**, **Extra Spaces**, and **Clip Signal** based on your encoding needs.
    * If you need to use a custom SAME header, check "Use custom SAME Header" and input your header in the text area.
3.  **Add Locations (Optional but Recommended):**
    * You can directly enter a **FIPS Code** and click "Add Location".
    * Alternatively, use the **State**, **County**, and **Region** dropdowns to select a location and then click "Add Selected Location".
    * Added locations will appear in the table below.
4.  **Generate and Play:**
    * Click the **"Generate"** button to create the EAS tones.
    * Click **"Play Samples"** to listen to the generated audio.
    * Click **"Save as wav file"** to download the audio.
    * If you want to clear the logs, click **"Clear Logs"**.

---

## Development

The project is structured with the following files:

* `index.html`: The main HTML structure of the application.
* `style.css`: Contains the CSS for styling the encoder's user interface.
* `audio.js`: Likely handles the audio generation and playback logic.
* `utils.js`: Contains utility functions used throughout the application.
* `dec.js`: Could be related to decoding or specific digital encoding aspects.
* `same.js`: Handles the SAME (Specific Area Message Encoding) header generation and processing.
* `alert.js`: Manages the alert generation flow.
* `main.js`: The primary JavaScript file orchestrating the application's logic.

---

## Credits

This EAS Encoder project builds upon the work of others. Special thanks to:

* [nicksmadscience/eas-same-encoder](https://github.com/nicksmadscience/eas-same-encoder) (Python SAME encoder)
* [Mab879/eas\_encoder](https://github.com/Mab879/eas_encoder) (C++ SAME encoder)
* [CryptoDude3](https://github.com/CryptoDude3) for the original 1.0 version of this project.
