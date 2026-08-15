# ChromeOS Update Engine Toggler (sysupd)

A lightweight utility script for ChromeOS to easily toggle, stop, and disable the system `update-engine` and its associated Upstart job configuration on-demand. This is particularly useful for managing dependent system services like Crostini/DLC components.

## Installation

You can deploy and install `sysupd` system-wide instantly using a single terminal command:

```bash
curl -sSL https://raw.githubusercontent.com/wicorn29/cOS-sysupd/main/sysupd | sudo tee /usr/local/bin/sysupd > /dev/null && sudo chmod +x /usr/local/bin/sysupd
```
> [!NOTE]
> I recommend you SSH into your chromebook and run the command from root there, so you don't have to type the entire string out in the virtual terminal.


## Usage

Run the command with sudo followed by your desired state (on or off):
Disable the update engine:
  ```Bash

  sudo sysupd off
  ```
    
  Enable and start the update engine:
  ```Bash

  sudo sysupd on
  ```
