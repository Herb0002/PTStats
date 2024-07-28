[![Downloads@latest](https://img.shields.io/badge/🪟%20Download%20Windows%20Version-0078D7?style=for-the-badge?style=for-the-badge)](https://github.com/Herb0002/PTStats/releases/latest/download/PTStats.exe)
[![Downloads@latest](https://img.shields.io/badge/🐧%20Download%20Linux%20Version-2C2C2C?style=for-the-badge?style=for-the-badge)](https://github.com/Herb0002/PTStats/releases/latest/download/PTStats.bin)


[![Downloads@all](https://img.shields.io/github/downloads/Herb0002/PTStats/total?style=for-the-badge&label=Downloads%20all&)](https://github.com/Herb0002/PTStats/releases)
[![Downloads@latest](https://img.shields.io/github/downloads/Herb0002/PTStats/latest/total?style=for-the-badge&label=Download%20latest%20Release)](https://github.com/Herb0002/PTStats/releases)
[![Downloads Version Badge](https://img.shields.io/github/v/release/Herb0002/PTStats?style=for-the-badge&label=Version:)](https://github.com/Herb0002/PTStats/releases) 

# **PTStats Installation and Usage:**

# Supported Platforms:
Windows: Windows 10 and aboven
Linux: x86_64 (AMD64) architecture

### For Linux:
Step 1: Make the File Executable First, you need to make sure the PTStats file is executable:
```
chmod +x PTStats.bin
```
 Step 2: Start the File in the Background Using nohup: To start the file in the background and ensure it keeps running after you close the terminal, use nohup: 
```
nohup ./PTStats.bin &
```
nohup: Prevents the process from stopping when the terminal is closed.
&: Runs the command in the background.

> Note: The updater supports nohup and pm2. A switch between these options is possible later through the dashboard. Ensure pm2 is installed and configured for autostart using the following commands (only if you are using pm2; skip this part if you are using nohup):


# Set up pm2 to run on startup
```
pm2 startup
```

# Start your application with pm2
```
pm2 start PTStats.bin --name PTStats
```

# Save the current process list, so it will start on reboot
```
pm2 save
```


Step 3: Access the Application

Locally: Open http://localhost:5000/login in your web browser. Remotely: Replace localhost with the server's IP address, e.g., http://DOMAIN:5000.

--- 
### For Windows: 
Step 1: Simply start the PTStats.exe file. Once the application is running, proceed to 

Step 2: Access the Application  
Locally: Open http://localhost:5000/login in your web browser. Remotely: Replace localhost with the server's IP address, e.g., http://DOMAIN:5000.

---
These steps should help you efficiently start and access your application. If you have any further questions or need additional details, feel free to ask!
