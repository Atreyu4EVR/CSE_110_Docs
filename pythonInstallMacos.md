# Installation Guide for Python on macOS

To install Python on macOS, you will need to use the Terminal application that comes pre-installed on your device from Apple. Using the Terminal application may seem foreign to you if you are not used to using the command line. Don't let this intimidate you though, Terminal is a powerful tool and I have broken down the steps to install Python on macOS into a few simple steps.

By following these steps, you will be able to install Python on your device in less than a minute. Terminal makes this process lightning fast and ensures that you have the latest version of Python installed on your device.

## Start by Opening Terminal

1. Type "Terminal" in the Spotlight search bar to locate it on your device.

2. From the search results, select the Terminal application.

## Steps to Install Python on macOS via Homebrew

In the terminal window, copy and paste the following commands, and press enter to run them. Take your time, and go through each step carefully.

1. **Install Homebrew**:

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Update Homebrew**: Before installing Python, update Homebrew to ensure you get the latest version of Python:

   ```bash
   brew update && brew upgrade
   ```

3. **Install the Latest Stable Release of Python**:

   ```bash
   brew install python
   ```

4. **Verify the Installation**: After installation, check the Python version to confirm it is installed correctly:

   ```bash
   python3 --version
   ```

Should return something like `Python 3.xx`, depending on most recent version available.

5. **Set Up PATH**: To ensure Python is correctly added to your PATH use the following command:

   ```bash
   echo 'export PATH="/usr/local/opt/python/libexec/bin:$PATH"' >> ~/.zprofile
   source ~/.zprofile
   ```

Congratulations! You have successfully installed Python on macOS.
