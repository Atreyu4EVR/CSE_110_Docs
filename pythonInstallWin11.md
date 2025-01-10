# Installation Guide for Python on Windows 11

To install Python on Windows 11, you will need to use the Windows PowerShell application that comes pre-installed on your device from Microsoft. Using the PowerShell application may seem foreign to you if you are not used to using the command line. Don't let this intimidate you though, PowerShell is a powerful tool and I have broken down the steps to install Python on Windows 11 into a few simple steps.

By following these steps, you will be able to install Python on your device in less than a minute. PowerShell makes this process lightning fast and ensures that you have the latest version of Python installed on your device.

## Start by Opening PowerShell

1. Type "PowerShell" in the search bar to locate it on your device.

2. From the search results, right click on PowerShell and select "Run as administrator".

## Install Chocolatey and Python

1. Run the following command to install Chocolatey:

   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
   ```

2. Once Chocolatey is installed, install Python by running:

   ```powershell
   choco install python -y
   ```

3. After installation, verify that Python is installed by typing:

   ```powershell
   python --version
   ```

   This should display the installed Python version.

Congratulations! You have successfully installed Python on Windows 11.
