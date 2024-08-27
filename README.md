[![Downloads@latest](https://img.shields.io/badge/🪟%20Download%20Windows%20Version-0078D7?style=for-the-badge?style=for-the-badge)](https://github.com/Herb0002/PTStats/releases/latest/download/PTStats.exe)
[![Downloads@latest](https://img.shields.io/badge/🐧%20Download%20Linux%20Version-2C2C2C?style=for-the-badge?style=for-the-badge)](https://github.com/Herb0002/PTStats/releases/latest/download/PTStats.bin)


[![Downloads@all](https://img.shields.io/github/downloads/Herb0002/PTStats/total?style=for-the-badge&label=Downloads%20all&)](https://github.com/Herb0002/PTStats/releases)
[![Downloads@latest](https://img.shields.io/github/downloads/Herb0002/PTStats/latest/total?style=for-the-badge&label=Download%20latest%20Release)](https://github.com/Herb0002/PTStats/releases)
[![Downloads Version Badge](https://img.shields.io/github/v/release/Herb0002/PTStats?style=for-the-badge&label=Version:)](https://github.com/Herb0002/PTStats/releases) 


![PT Stats Logo](https://cdn.discordapp.com/attachments/1056301681190654083/1277610537211138140/ptaddon.2fa95fea.png?ex=66cdcb08&is=66cc7988&hm=8dac1b3a0bf5535ffe6e90f03cdebdd525074f4b92e2be87e11e38fb1b0e877b&)

PT Stats is an authorized add-on to ProfitTrailer, one of the best crypto trading bots. However, it is developed and supported by a different team, so the ProfitTrailer support channels will not be able to provide any support information about this tool.

For any assistance or inquiries regarding PT Stats, please feel free to join the ProfitTrailer Discord server. There is a dedicated channel named **PTStats** where you can ping me, **Herb**, directly for help or to ask questions.


# **PTStats Installation and Usage:**

**Supported Platforms:**
- **Windows**: Windows 10 and above
- **Linux**: x86_64 (AMD64) architecture, requires GLIBC 2.37 or higher


### For Linux:

Step 1: Update Your System

Before proceeding with the installation, it is recommended to update your system to ensure all packages are up-to-date:

```
sudo apt update
sudo apt upgrade -y
```

Step 2: Make the File Executable First, you need to make sure the PTStats file is executable:
```
chmod +x PTStats.bin
```
Step 3: Choose a Method to Run the Application in the Background
You can use either nohup or pm2 to run the application in the background.

Option 1: Using nohup
To start the file in the background and ensure it keeps running after you close the terminal, use:

```
nohup ./PTStats.bin &
```
nohup: Prevents the process from stopping when the terminal is closed.
&: Runs the command in the background.

Option 2: Using pm2
If you prefer using pm2, ensure it is installed and configured for autostart:

Set up pm2 to run on startup:
```
pm2 startup
```

Start your application with pm2:
```
pm2 start PTStats.bin --name PTStats
```

Save the current process list, so it will start on reboot:
```
pm2 save
```
> Note: You only need to use one of these methods (nohup or pm2). You can switch between them later through the dashboard if necessary.


Step 4: Access the Application

Locally: Open http://localhost:5000/login in your web browser. Remotely: Replace localhost with the server's IP address, e.g., http://DOMAIN:5000/login.

--- 
### For Windows: 
Step 1: Simply start the PTStats.exe file. Once the application is running, proceed to 

Step 2: Access the Application  
Locally: Open http://localhost:5000/login in your web browser. Remotely: Replace localhost with the server's IP address, e.g., http://DOMAIN:5000/login.

---
These steps should help you efficiently start and access your application. If you have any further questions or need additional details, feel free to ask!
