# WiFi Credentials Harvester

---

## Description

The **WiFi Credentials Harvester** is a payload designed for educational and ethical purposes. It targets Windows systems to extract saved Wi-Fi network credentials, including the associated passwords, and securely copies them to the Bash Bunny's storage for review.

This payload demonstrates how Wi-Fi credentials can be easily accessed on machines that store network profiles, emphasizing the importance of securing sensitive information.

## How it Works

1. The payload launches PowerShell with administrator privileges on a Windows machine.
2. It uses the `netsh wlan` command to export all stored Wi-Fi profiles, including passwords in clear text.
3. The profiles are saved as XML files in a publicly accessible directory.
4. The payload then copies these XML files to the Bash Bunny's storage device.
5. Finally, PowerShell is exited, and the Bash Bunny can be safely removed.

## Requirements

- Target: Windows machine with saved Wi-Fi credentials
- Bash Bunny in HID and storage mode

## Ethical Use Disclaimer

This payload is developed for ethical hacking and educational purposes only. Unauthorized use of this script to access Wi-Fi credentials on any device without explicit permission is illegal and unethical. Always ensure you have proper authorization before running this script.

## Liability Disclaimer

The author of this payload assumes no responsibility for any illegal or unethical use of the code. This payload is provided as-is, and it is the user's responsibility to ensure its use complies with all applicable laws and regulations.

## Usage

1. Insert the Bash Bunny into the target machine.
2. Wait for the script to execute and retrieve the Wi-Fi credentials.
3. Safely eject the Bash Bunny and access the saved credentials from the `/wifi_profiles` directory.
