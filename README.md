
![PT Stats Logo](Logo.png)

[![Download PTStats.zip](https://img.shields.io/badge/⬇️%20Download%20PTStats.zip-4C1?style=for-the-badge)](https://github.com/Herb0002/PTStats/releases/latest/download/PTStats.zip)
[![Total Downloads](https://img.shields.io/github/downloads/Herb0002/PTStats/total?style=for-the-badge&label=Downloads%20All)](https://github.com/Herb0002/PTStats/releases)
[![Latest Release](https://img.shields.io/github/downloads/Herb0002/PTStats/latest/total?style=for-the-badge&label=Download%20Latest%20Release)](https://github.com/Herb0002/PTStats/releases)
[![Version](https://img.shields.io/github/v/release/Herb0002/PTStats?style=for-the-badge&label=Version:)](https://github.com/Herb0002/PTStats/releases)

PT Stats is an authorized add-on to ProfitTrailer, one of the best crypto trading bots. However, it is developed and supported by a different team, so the ProfitTrailer support channels will not be able to provide any support information about this tool.

For any assistance or inquiries regarding PT Stats, please feel free to join the ProfitTrailer Discord server. There is a dedicated channel named **PTStats** where you can ping me, **Herb**, directly for help or to ask questions.

# **PTStats Installation and Usage:**

## Table of Contents
1. [Supported Platforms](#supported-platforms)
2. [For Linux](#for-linux)
    - [Update Your System](#update-your-system)
    - [Make the File Executable](#make-the-file-executable)
    - [Run the Application in the Background](#run-the-application-in-the-background)
    - [Access the Application](#access-the-application)
3. [For Windows](#for-windows)
    - [Start the Application](#start-the-application)
    - [Access the Application](#access-the-application)

## Supported Platforms:
- **Windows**: Windows 10 and above
- **Linux**:
  - **x86_64 (AMD64)** architecture, requires GLIBC 2.37 or higher
  - **ARM** architecture, requires GLIBC 2.37 or higher

### For Linux:

#### Update Your System
Before proceeding with the installation, it is recommended to update your system to ensure all packages are up-to-date:

```
sudo apt update
sudo apt upgrade -y
```

#### Make the File Executable
First, you need to make sure the PTStats file is executable:
```
chmod +x PTStats.bin
```

#### Run the Application in the Background
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

### Access the Application

#### Locally
- Open [http://localhost:5000](http://localhost:5000) in your web browser.

#### Remotely
- Replace `localhost` with your server's domain name or IP address, e.g., [https://DOMAIN:5000](https://DOMAIN:5000).

**Best Practice:** It is recommended to use a domain with **SSL** (HTTPS). Accessing the application without SSL is **not recommended**.

---

### For Windows:

#### Start the Application
- Simply start the `PTStats.exe` file. Once the application is running, proceed to:

### Access the Application

#### Locally
- Open [http://localhost:5000](http://localhost:5000) in your web browser.

#### Remotely
- Replace `localhost` with the server's IP address or domain, e.g., [https://DOMAIN:5000](https://DOMAIN:5000).

**Best Practice:** It is recommended to use a domain with **SSL** (HTTPS). Accessing the application without SSL is **not recommended**.

---
These steps should help you efficiently start and access your application. If you have any further questions or need additional details, feel free to ask!
