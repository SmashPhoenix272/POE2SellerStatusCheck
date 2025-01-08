POE2 Seller Status Check Userscript

## Description

This userscript monitors seller status on the Path of Exile 2 trade site (pathofexile.com/trade2) and provides notifications when sellers come online. It adds an "Alert" button next to the "Refresh" button for each item listing, allowing you to track specific sellers and receive audio alerts when they change their status from Offline or AFK to Online.

## Features

-   **Status Monitoring:** Tracks the online status of sellers (Online, Offline, and AFK).
-   **Alert Button:** Adds an "Alert" button to each item listing for easy monitoring.
-   **Audio Notifications:** Plays a customizable sound alert when a monitored seller comes online.
-   **Repeated Alerts:** Repeats the alert every 5 minutes if the seller is still online since the last alert.
-   **Customizable Configuration:** Allows you to adjust the following settings:
    -   Check interval (how often the script checks for status changes)
    -   Alert sound type
    -   Volume (with a warning for values above 1.0 that may cause distortion)
    -   Sound duration
    -   Sound repeat count

## Installation

1. Install a userscript manager extension for your browser:
    -   **Tampermonkey:** [https://www.tampermonkey.net/](https://www.tampermonkey.net/)
    -   **Violentmonkey:** [https://violentmonkey.github.io/](https://violentmonkey.github.io/)
2. Copy the contents of the `poe2_seller_status.user.js` file.
3. Open your userscript manager's dashboard and create a new script.
4. Paste the copied code into the new script.
5. Save the script.

## Configuration

After installing the userscript, you can access the configuration panel by clicking on the userscript manager's icon in your browser toolbar and selecting "POE2 Seller Status Check Configuration" from the menu.

The following options are available:

-   **Check Interval (ms):** The time interval (in milliseconds) between status checks. The default is 30000 (30 seconds).
-   **Alert Sound:** The type of sound to play for the alert. Options include "Alert 1" (High Beep), "Alert 2" (Double Tone), and "Alert 3" (Musical).
-   **Volume:** The volume of the alert sound (ranging from 0 to potentially above 1). **Warning:** Values above 1 may cause audio distortion.
-   **Sound Duration (ms):** The duration of the alert sound in milliseconds.
-   **Sound Repeat Count:** The number of times to repeat the alert sound.

## Usage

1. Navigate to the Path of Exile 2 trade site: [https://www.pathofexile.com/trade2/search/poe2/](https://www.pathofexile.com/trade2/search/poe2/)
2. Search for the items you want to monitor.
3. For each item listing, click the "Alert" button next to the "Refresh" button for the sellers you want to track. The button will turn red when active.
4. The script will periodically check the status of the monitored sellers.
5. When a monitored seller changes their status from Offline or AFK to Online, you will receive an audio notification.
6. The notification will repeat every 5 minutes as long as the seller remains online.

## Troubleshooting

-   **AudioContext Error:** If you encounter an error related to the `AudioContext`, make sure you interact with the page (e.g., click anywhere) after installing the userscript. This is a browser security requirement to prevent unwanted autoplay of audio. You can also test the sound in the configuration panel to ensure the `AudioContext` is properly initialized.
-   **No Notifications:** If you are not receiving notifications, make sure that:
    -   The userscript is enabled in your userscript manager.
    -   The "Alert" button is active (red) for the sellers you want to monitor.
    -   The volume on your computer is turned up.
    -   The configuration options are set correctly.

## Contributing

Contributions to this userscript are welcome. Please feel free to submit pull requests or open issues on the project's repository (if available).

## License

This project is licensed under the [MIT License](LICENSE) (replace with your chosen license and add a LICENSE file if applicable).
