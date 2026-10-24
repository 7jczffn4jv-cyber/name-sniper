# Discord user name checker and generator
A high-speed, infinite Discord username generator and checker. Built for Linux and Windows shells with proxy rotation and instant webhook alerts.

✔️ **INSTALLATION LINUX/MAC:**

git clone https://github.com/yourusername/name-sniper.git

cd name-sniper

sudo apt-get update

sudo chmod +x install.sh

sudo bash install.sh


#!/bin/bash
echo "[*] Updating package lists..."
sudo apt-get update -y

echo "[*] Checking Python installation..."
if ! command -v python3 &> /dev/null; then
    echo "[!] Python3 not found. Installing..."
    sudo apt-get install python3 python3-pip -y
else
    echo "[+] Python3 is installed."
fi

echo "[*] Installing required libraries..."
pip3 install -r requirements.txt

echo "[+] Installation complete. Run 'python3 sniper_linux.py' to start."
✔️ **INSTALLATION LINUX/MAC (Venv Enviroment):**

If you encounter some errors in the python libraries installation use this method

git clone https://github.com/yourusername/name-sniper.git

sudo apt-get update


cd name-sniper

python3 -m venv .lib_venv

sudo chmod +x install.sh

sudo bash install.sh

source .lib_venv/bin/activate

pip3 install -r requirements.txt


python3 sniper_linux.py


✔️ **INSTALLATION WINDOWS (1°WAY)**

If you have git installed on your windows machine you can do the following commands:

git clone https://github.com/yourusername/name-sniper.git

cd name-sniper

Install.cmd

✔️ **INSTALLATION WINDOWS (2° WAY)**

If you download the zip file of Name-Sniper you should first unzip it and after that do the following commands:

ren name-sniper-main name-sniper
cd name-sniper
Install.cmd

@echo off
echo [*] Checking Python installation...
python --version >nul 2>&1
if %errorlevel% neq 0 (
    echo [!] Python is not installed or not in PATH. Please install Python from python.org
    pause
    exit /b
)

echo [*] Installing required libraries...
pip install -r requirements.txt

echo [+] Installation complete. Run 'python sniper_win.py' to start.
pause

✔️ **INSTALLATION TERMUX:**

pkg install python
pkg install git
git clone https://github.com/yourusername/name-sniper.git
cd name-sniper
pip install -r requirements.txt

**USAGE LINUX/MAC:**

cd name-sniper
python3 sniper_linux.py

**USAGE LINUX/MAC (Venv Enviroment):**

cd name-sniper
source .lib_venv/bin/activate
python3 sniper_linux.py

**USAGE TERMUX:**

python sniper_linux.py

**USAGE WINDOWS:**

python sniper_win.py

---
**DISCLAIMER**

This tool is for educational purposes only. Discord's API rate-limits unauthenticated requests heavily. You may need to supply an Authorization token in the headers if proxies are not enough. The developer is not responsible for any misuse or account bans. Use at your own risk.
