# P1Touch Screen

## Table of Contents

1. [Introduction](#1.-introduction)
2. [Features](##2.-features)
3. [Installation](##3.-installation)
   - [Install Drivers](#install-drivers)
   - [Prepare the SD card](#prepare-the-sd-card)
   - [Online Web Installer](#online-web-installer)
   - [Linking Printer](#linking-printer)
4. [Screens](#4.-screens)
   - [Main](#main-screen)
   - [Temperature / Fan](#temperature--fan-screen)
   - [Control](#control-screen)
   - [Filament](#filament-screen)
   - [Settings](#settings-screen)
5. [OTA Update Procedure](#5.-ota-update-procedure)

---

## 1. Introduction

The P1Touch Screen is a revolutionary addition to your BambuLab Printer, enhancing the user experience and providing advanced control and monitoring capabilities. This detailed README.md guide will walk you through the product's features, installation process, and the functionality of different screens.

## Required Hardware

Currently, it has only been tested on the affordable 2.8-inch ESP32-2432S028R board, which is available for purchase here:

![image](https://github.com/xperiments/p1touch/assets/417709/28bdca76-9e49-4aab-a4c1-b714546077b4)
![image](https://github.com/xperiments/p1touch/assets/417709/658061e4-d638-4d1e-ab99-268baba40ebc)

[https://fr.aliexpress.com/item/1005004502250619.html](https://fr.aliexpress.com/item/1005004502250619.html)

## 2. Features

- **Advanced Touch Screen**: A touch screen interface for intuitive printer control.
- **Status Indicators**: Top bar indicating WiFi connectivity, camera status, timelapse recording, and AMS status.
- **Temperature Monitoring**: Real-time display of nozzle, bed, and chamber temperatures.
- **Printing Control**: Full control over your print job, including the ability to change print speed during printing.
- **Precise Control**: Control your printer's XYZ position with adjustable head movement steps (1mm and 10mm).
- **Filament Handling**: Load, unload, extrude, and retract filament (Note: Filament handling available only for printers without AMS initially).
- **Customizable Settings**: Access a wide range of LCD and printer-related settings.
- **OTA Updates**: Enable over-the-air updates for firmware enhancements.

## 3. Installation

### Install Drivers

[Install CH340 Drivers](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all)

### Prepare the SD card

Before you begin the installation process for the P1Touch Screen, it's essential to properly initialize your SD card with the necessary configuration for connecting to your WiFi network. Follow these steps carefully:

1. **Format the SD Card in FAT32**:

   - Ensure your SD card is formatted with the FAT32 file system. You can use your computer's built-in formatting tools or third-party software to format the card if needed.

2. **Create a Configuration File**:

   - On the root directory of the SD card, create a JSON configuration file named `wifi.json`. You can use a plain text editor to create this file.

3. **Edit the Configuration File**:
   - Open the `wifi.json` file in a text editor and replace the following placeholders with the actual information for your WiFi network:

```json
{
  "ssid": "your_ssid_name",
  "pwd": "your_ssid_password"
}
```

Replace `"your_ssid_name"` with your WiFi network's SSID (name) and `"your_ssid_password"` with your WiFi network's password.

4. **Save the Configuration File**:
   - Save the changes you made to the `wifi.json` file.

Your SD card is now properly initialized with the required WiFi configuration. This configuration will enable the P1Touch Screen to connect to your WiFi network during the installation process. Ensure that the SD card is securely inserted into the touch screen before proceeding with the installation steps outlined in the previous sections of this README.md file.

Certainly, here's an addition to the installation section of your README.md file explaining the Online Web Installer process:

### Online Web Installer

To set up your P1Touch Screen, you will need to use the Online Web Installer. Follow these steps to complete the installation:

1. **Open a Web Browser**:

   - Open your preferred web browser on a computer.

2. **Enter the Web Installer URL**:

   - In the browser's address bar, enter the following URL:
     ```
     CLOSED BETA
     ```

3. **Connect Button**:

   - On the web page, locate and click the "Connect" button to establish a connection between your computer and the P1Touch Screen.

4. **Select P1Touch Serial Port**:

   - After clicking "Connect," a list of available serial ports will be displayed. Choose the one asigned to your P1Touch to establish a connection with the touch screen.

5. **Install P1Touch**:

   - Once you've selected the correct serial port, click the "Install P1Touch" button on the web page. This will initiate the installation process.

6. **Installation Completion**:

   - Wait for the installation to complete. You will receive a confirmation message or indication on the web page once the installation process finishes.

7. **Power Off the Screen**:

   - Turn off the P1Touch Screen.

8. **Insert the Prepared SD Card**:

   - Place the SD card prepared with the required configuration (as explained earlier) back into the P1Touch Screen.

9. **Power On the Screen**:

   - Turn on the P1Touch Screen. It will now be fully initialized and ready for use with your 3D printer.

Thank you for providing additional details. Here's the updated explanation for the "Linking Printer" section in your README.md file:

### Linking Printer

During the installation process, you will need to link your P1Touch Screen with your 3D printer. Follow these steps to successfully establish the connection:

1. **Searching for Printers**:

   - After powering on the touch screen, you will be greeted with a "Searching for printers" screen. The touch screen will scan the network for available printers.

2. **Select a Printer to Link**:

   - Once the scanning process is complete, you will be presented with a listing of the printers that were found on the network. Select the printer you wish to link.

3. **Click the Checkmark Button**:

   - After selecting the desired printer, click the green checkmark button to initiate the linking process.

4. **Enter the Access Code**:

   - You will be prompted to enter the access code for the selected printer. Provide the correct access code and proceed.

5. **Connecting to the Printer**:

   - The P1Touch Screen will attempt to establish a connection with the selected printer. If the connection is unsuccessful, the process will restart, allowing you to try again.

6. **Success and Main Screen**:

   - Upon successfully linking the touch screen with the printer, you will be redirected to the Main Screen. Your printer and touch screen are now connected and ready for use.

7. **Saving Access Code**:

   - The access code for the linked printer will be saved for future use. This means that for subsequent printer links (if the printer is the same), you will not be asked for the access code again. You can clear these saved access codes in the Settings Screen if needed.

By following these steps, you will be able to link your P1Touch Screen with your 3D printer seamlessly, ensuring a smooth user experience and easy access to all the features of the touch screen.

Please ensure that the access code is kept secure and that you clear the access code cache in the Settings Screen if you wish to unlink the printer or start the linking process for a different printer.

## 4. Screens

### Main Screen

- **Top Bar**: Displays WiFi, camera, timelapse, and AMS status.
- **Light Control**: Toggle the printer's light on/off.
- **Temperature Indicators**: Real-time nozzle, bed, and chamber temperature indicators.
- **Status Area**: Shows a "Ready" message when the printer is idle; during printing, it displays print control buttons, progress, and estimated time. Allows real-time print speed adjustment.

### Temperature / Fan Screen

- **Temperature Indicators**: Display nozzle, bed, and chamber temperatures.
- **Temperature Adjustment**: Tap on any indicator to change the temperature or fan speed.

### Control Screen

- **Homing**: Home the printer.
- **XYZ Position Control**: Precise control over the print head's XYZ position.
- **Step Size**: Switch between 1mm and 10mm head movement steps.

### Filament Screen

- **Filament Handling**: Load, unload, extrude, and retract filament (Note: Filament handling available only for printers without AMS initially).

### Settings Screen

#### LCD

- **Change Backlight**: Adjust the screen backlight.
- **Set Screen Sleep Time**: Configure the screen's sleep time (set to 0 to disable).
- **Invert Screen Colors**: Toggle screen color inversion.
- **Flip Screen**: Flip the screen orientation.

#### PRINTERS

- **Unlink Printer**: Disconnect the printer from the touch screen.
- **Clear Access Code Cache**: Remove cached printer access codes.

#### XTOUCH

- **AUX FAN**: Enable the auxiliary fan for printers that initially lack it.
- **CHAMBER Temp**: Enable chamber temperature monitoring for printers without it.
- **OTA Update**: Enable OTA upgrades for firmware updates.

Certainly, here's the updated explanation for the "OTA Update Procedure" section in your README.md file:

## 5. OTA Update Procedure

The P1Touch Screen supports Over-The-Air (OTA) firmware updates, making it easy to keep your device up to date with the latest features and improvements. To enable and utilize OTA updates, follow these steps:

1. **Access the Settings Screen**:

   - Navigate to the Settings Screen on your P1Touch Screen.

2. **Enable OTA Updates**:

   - In the Settings Screen, locate the OTA Update section. You will find an option to enable OTA updates. Toggle this option to "ON" to enable automatic firmware update checks.

3. **Automatic Update Check on Boot**:

   - With OTA updates enabled, your touch screen will automatically check for firmware updates every time it boots up.

4. **Download and Apply Updates**:

   - If an update is available, the touch screen will automatically download the latest firmware and apply the upgrade. This process is seamless and requires no manual intervention.

By enabling OTA updates in the Settings Screen, you ensure that your P1Touch Screen stays current with the latest software enhancements and bug fixes without the need for manual updates. This convenient feature ensures that you always have access to the best performance and functionality that the device can offer.

Certainly, here's the explanation for the standard firmware update procedure in your README.md file:

## 6. Standard Firmware Update

If you prefer to manually update the firmware of your P1Touch Screen or if OTA updates are not enabled, you can follow this procedure:

1. **Download the Update Firmware File**:

   - Visit the official P1Touch website or the designated firmware update source to download the latest firmware update file. Ensure that you download the file with the `firmware.bin` name.

2. **Copy the Firmware File to the Root of the SD Card**:

   - Insert the SD card into your computer's card reader.
   - Copy the downloaded firmware update file `firmware.bin` to the root directory of the SD card. Do not place it in any subdirectories.

3. **Reboot the P1Touch Screen**:

   - Insert the SD card containing the firmware update file into the P1Touch Screen if it's not already inserted.

   - Reboot the touch screen. You can do this by turning it off and then turning it back on.

4. **Apply the Firmware Update**:

   - Once the touch screen has booted up, it will detect the presence of the firmware update file on the SD card.

   - The touch screen will apply the firmware update.

   - The update process may take a few minutes to complete. Do not turn off the touch screen or remove the SD card during this time.

5. **Completion and Verification**:

   - After the firmware update is successfully applied, the touch screen will notify you that the update is complete.

   - You can verify the firmware version in the touch screen's settings section to ensure that it matches the latest version.

By following these steps, you can manually update the firmware of your P1Touch Screen to the latest version, ensuring that you have access to all the latest features and improvements.
