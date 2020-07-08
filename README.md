# Open Source EDA Tools used to design the IP
``` LTSpice XVII ```

``` Ngspice ```

``` Magic VLSI```

## Steps to install ``` LTSpice XVII ``` on LINUX
1. It`s not directly supported, so we need to download ```WineHQ```. Wine is a linux software that creates windows environment and allows you to run various windows programs.
2. Copy paste the commands mentioned below one after the other in the terminal for downloading and installing.
``` 
sudo dpkg --add-architecture i386
wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -
sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'
sudo apt update
sudo apt install --install-recommends winehq-stable
```
3. Download [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html).
4. Click on ```Download for Windows```.
5. Install it by clicking on ``` -> next ```.
6. After installing , click on open with ```WineHQ windows program loader```.
``` LTSpice is now installed and you can design the circuit```
## Steps to install ```Ngspice``` on LINUX
It’s Super Easy! simply click on Copy button to copy the command and paste into your command line terminal using built-in APT package manager.

1. Run update command to update package repositories and get latest package information ```sudo apt-get update -y```
2. Run the install command with -y flag to quickly install the packages and dependencies ```sudo apt-get install -y ngspice```
3. Check the system logs to confirm that there are no related errors.

Note: ```-y```flag means to assume yes and silently install, without asking you questions in most cases

### Steps to install ```Magic VLSI``` on LINUX
1. Download the [magic.sh file](https://drive.google.com/file/d/1F0y1xuYWIgeYEpzKnGlaCQH3urdSFc4E/view)
2. Copy paste the below commands one after another
``` 
cd Downloads/
chmod +x magic.sh
./magic.sh

```
* Magic tool will be opened with minimum technology file by default but we have to use osu180nm tech file. Follow below steps to open magic with osu180nm tech file.
3. Download the ```osu180nm.tech``` file from the uploaded files. Copy and paste the entire content in ```Text Editor``` and save it as ```osu180nm.tech```.
4. Open the Terminal and copy, paste the commands mentioned below.
```
sudo cp osu180nm.tech /usr/local/lib/magic/sys/
cd /usr/local/lib/magic/sys/
ls 
cd
clear
```
* You have successfully added osu180nm.tech file!
* Just open the terminal and type ```magic -T osu180nm.tech``` .











