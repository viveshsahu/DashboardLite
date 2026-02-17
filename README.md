# DashboardLite
Dashboard Application to display running status of all the networks supported devices available on the local network

<img width="1216" height="860" alt="DashboardLite_UI2" src="https://github.com/user-attachments/assets/18339b73-f11b-49b8-a103-bb7dac1d3f1e" />

# Hosting
Windows - Run the 'DashboardLite.exe' to start the application. The 'DashboardLite.exe' can be added to 'Startup Apps' to auto launch the application at system boot.

Linux - Run './DashboardLite' to start the application. User can create a system service using 'systemctl' to host the application as a service.

Raspberry Pi - Run './DashboardLite' to start the application. User can create a system service using 'systemctl' to host the application as a service.

# Configuration
User needs to modify 'appsettings.json' file to configure all the devices running on the local network.


AppConfiguration": {
    "DashboardTitle": "",
    "City": "Bhubaneshwar",
    "Devices": [
      {
        "DeviceName": "Mini PC",
        "DeviceIPAddress": "192.168.0.105",
        "DeviceIcon": "/icons/minipc.png"
      },
      {
        "DeviceName": "RPI",
        "DeviceIPAddress": "192.168.0.123",
        "DeviceIcon": "/icons/rpi.jpg"
      } ]

urls - Specify the Url for the application.

DeviceName - Displays the device name when user hovers on the device icon.

DeviceIPAddress - The IP address for the particular device. It needs to be configured as a static IP on the router.

DeviceIcon - The icon for a particular device needs to be stored in 'icons' folder and link for the same needs to be added. 

