# Open Source EDA Tools used to design the IP
``` LTSpice XVII ```
``` Ngspice ```
``` Magic ```

### Installation Steps 
> Steps for installaton of ``` LTSpice XVII ``` in LINUX
1. It`s not directly supported, so we need to download ```WineHQ```
2. Copy paste the commands mentioned below one after the other in the terminal for downloading and installing.
``` 
sudo dpkg --add-architecture i386
wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -
sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'
sudo apt update
sudo apt install --install-recommends winehq-stable
```
3. Download [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html).
4. Click on ```Donload for Windows```.
5. Install it by clicking on ``` -> next ```.
6. After installing , click on open with ```WineHQ windows program loader```.

