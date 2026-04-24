---
title: Getting Started
description:  A comprehensive guide to adding devices, managing device information, and flashing firmware within the SenseCraft HMI platform.
---


Before using SenseCraft HMI, it is highly recommended to update your device firmware to the latest version. This ensures optimal performance, bug fixes, and access to the latest features.

---

## Add a New Device
1. **Enter Config Mode**: By default, new devices (or those after a Full Flash) enter configuration mode upon startup.
2. **Connect to Device Wi-Fi**: Use your smartphone or PC to connect to the Wi-Fi hotspot displayed on the ePaper screen.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/reterminal_e10xx/img/5.png" style={{width:400, height:'auto'}}/></div><br />

3. **Access Config Page**: Open a browser and go to `http://192.168.4.1/`.
4. **Configure Network**: Select your local Wi-Fi, enter the password, and click **Connect**.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/reterminal_e10xx/img/6.png" style={{width:700, height:'auto'}}/></div><br />

5. **Get Pairing Code**: Once connected, the device will automatically display a **6-digit pairing code**.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/reterminal_e10xx/img/136.png" style={{width:600, height:'auto'}}/></div>

6. **Add to Platform**: In the SenseCraft HMI **Device** page, click **+ Add NEW Device**.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_4.png" style={{width:600, height:'auto'}}/></div><br />

7. **Finalize Pairing**: Enter a custom name for your device and the 6-digit pairing code, then click **Create**.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/reterminal_e10xx/img/8.png" style={{width:600, height:'auto'}}/></div>

### Device-Specific Setup Guides
For more detailed network setup instructions, refer to:
* **reTerminal E1001**: [Network Setup Guide](https://wiki.seeedstudio.com/getting_started_with_reterminal_e1001/#network-setup)
* **reTerminal E1002**: [Network Setup Guide](https://wiki.seeedstudio.com/getting_started_with_reterminal_e1002/#network-setup)

---

## Device Information
On the **Device** page, you can view basic device information, including the **Device Name** and **Battery Level**.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_5.png" style={{width:600, height:'auto'}}/></div><br />

### Detailed Management
Click on a device to open the **Details** view. At the top of the panel, you can monitor and modify various settings, including:
* **Low Power Mode**: Toggle energy-saving settings.
* **Refresh Interval**: Adjust how often the screen updates.
* **Online Status**: Real-time connectivity tracking.
* **Battery Status**: Current power percentage.
* **Active Page**: View and manage the content currently displayed on the screen.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_6.png" style={{width:600, height:'auto'}}/></div><br />




---

## Firmware Flashing
Before you begin, ensure you have:
* **USB Cable**: To connect your device to your computer.
* **Stable Internet**: For downloading firmware files.
* **Modern Browser**: Chrome, Firefox, Safari, or Edge recommended.
* **Device Power**: Ensure your device has sufficient power.
### Step 1: Access the Firmware Flasher
1. Log in to your [SenseCraft HMI](https://sensecraft.seeed.cc/hmi) account.
2. Navigate to the **Tools** tab.
3. Click the **Firmware Flasher** button located at the top of the screen.

### Step 2: Select Your Device
1. Connect your device to your computer via USB.
2. Click the **Select** button.
3. A modal will appear; choose your device from the list of supported hardware.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_1.png" style={{width:600, height:'auto'}}/></div><br />

:::note
If you select the **ePaper DIY Kit - EE04**, you must also select the specific screen type and size you are using to ensure the correct display drivers are included.
:::

### Step 3: Select Firmware
1. Click the dropdown menu under **Select firmware**.
2. Choose the version you wish to install
3. **Optional**: Click **Connect Serial Monitor** if you need to view debug logs during the process.

<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_2.png" style={{width:600, height:'auto'}}/></div><br />

### Step 4: Flash the Firmware
1. Click the **Flash** button to begin.
2. **Important**: Do not disconnect the device or close the browser tab until the progress bar reaches 100%.
3. **Full Flash vs. Standard Flash**<br />
**Standard Flash (Unchecked)**: Updates firmware but preserves Wi-Fi credentials and settings. Recommended for regular updates.<br />
**Full Flash (Checked)**: Erases the **entire** memory. This will delete your Wi-Fi password and settings. Recommended for troubleshooting or factory resets.


<div style={{textAlign:'center'}}><img src="https://files.seeedstudio.com/wiki/hmi/img/hmi_getting_started_3.png" style={{width:600, height:'auto'}}/></div><br />


### After Flashing
1. Wait for the device to restart automatically.
2. If you performed a **Full Flash**, you will need to reconfigure Wi-Fi and re-pair the device.