# zundernet windows install instruction
⚠️ backup your wallet before proceeding ⚠️
### install dependencies

Get python3 from the official website [here](https://www.python.org/downloads/)
**Add python to $PATH** (in order to run python from cmd or powershell)

![Add Python to path](https://pasteimg.com/images/2021/07/28/py.png)

At the very end of the install process, allow +256 length commands to ensure nothing will break if encounters long commands.

Once Python is installed, we need to install some dependencies.

Open a PowerShell by hitting simultaneously **Win + R** and type "**powershell**"

![Run PowerShell](https://pasteimg.com/images/2021/07/28/run.png)

Then, copy and paste the following command and hit **Enter**

```
pip3 install pycryptodome; pip3 install pyside2; pip3 install psutil
```

![pip3 dependencies powershell](https://pasteimg.com/images/2021/07/28/pip3xyz.png)

Now you'll need to install the PirateChain CLI for windows [here](https://github.com/PirateNetwork/pirate/releases/download/v5.2.0/pirate-windows-v5.2.0.zip)
Unzip it and **keep it's path in mind**

Install TreasureChest as well if not done already [here](https://github.com/PirateNetwork/pirate/releases/download/v5.2.0/pirate-qt-windows-v5.2.0.zip)

Unzip and run it, it will sync the blockchain
**This might takes time if that's your 1st install**
You may want to speed up this process by downloading the bootstrap file [here](http://bootstrap.dexstats.info/ARRR-bootstrap.tar.gz)

Then delete everything in this repository then unzip the bootstrap here :

```
C:\Users\[YOUR_USERNAME]\AppData\Roaming\Komodo\Pirate
```

The "AppData" folder might me hidden by default, to see it press simultaneously **Win + R** and type

```
control.exe folders
```

![run folders options](https://pasteimg.com/images/2021/07/28/runfolders.png)

then, click one the "**View**" tab, and check the radio button "**Show hidden files, folders and drives**"

![display hidden files and folders in windows](https://pasteimg.com/images/2021/07/28/runfolders2.png)

You're now able to see the **AppData** folder.

If you encounter this warning, just click here :

![Windows Warining](https://pasteimg.com/images/2021/07/28/win.png) 

![Windows Warining](https://pasteimg.com/images/2021/07/28/winallow.png)

Once both arrr installed, download zundernet [here](https://github.com/buidl1/zundernet/archive/refs/heads/main.zip)

Unzip it, then open it and hodl **shift** while right clicking on the zundernet-main folder to "Open PowerShell window here" 
![Open PowerShell window here](https://pasteimg.com/images/2021/07/28/powershellhere.png)

Then run this command :

```
python zundernet.py
```
You'll be prompted to locate both Komodo and Data paths
![zundernet windows](https://pasteimg.com/images/2021/07/28/zunderwin.png)

The Komodo path is where you unzipped pirate-cli, while the data directory is a bit more tricky..

```
C:\Users\[YOUR_USERNAME]\AppData\Roaming\Komodo\PIRATE
```

Then, you'll be prompted to enter a password :

![zundernet prompt password](https://pasteimg.com/images/2021/07/28/zundernetpwd.png)

Now you're in, click "**Start Blockchain**" to start the deamon

![zundernet UI](https://pasteimg.com/images/2021/07/28/zundernetfinal.png)

Congratulations, You did it !!! 👏👏👏
