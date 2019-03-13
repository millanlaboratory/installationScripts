## <span id="Loop"> Loop </span>
**OS tested**: Ubuntu 14.04 LTS & 16.04 LTS (laptop & desktop), Ubuntu 18.04 LTS & 19.04 (desktop only)

**Duration**: 1h30min if MATLAB was not installed beforehand, 15min otherwise.

**After installation, these packages will be installed:**
autoconf
cifs-utils
[cnbitkextra](https://github.com/millanlaboratory/cnbitkextra),
[cnbitkloop](https://github.com/millanlaboratory/cnbitkloop),
[cnbi-smrtrain](https://github.com/millanlaboratory/cnbi-smrtrain),
[drawtk](https://github.com/millanlaboratory/drawtk),
[eegc](https://github.com/millanlaboratory/eegc),
[eegdev](https://github.com/millanlaboratory/eegdev),
[eegview](https://github.com/millanlaboratory/eegview),
flex
gcc-4.8
git
gnulib
libusb-1.0-0-dev
libfreetype6-dev
libfontconfig1-dev
libgstreamer0.10-0
libxml2-dev
libgstreamer-plugins-base0.10-dev
libsdl1.2-dev
libsdl-image1.2-dev
libsdl-ttf2.0-dev
libfreeimage-dev
libgtk2.0-dev
[lpttrigger](https://github.com/millanlaboratory/lpttrigger),
[mcpanel](https://github.com/millanlaboratory/mcpanel),
mwrap
MATLAB R2017b
python2.7
[rtfilter](https://github.com/millanlaboratory/rtfilter),
[tobicore](https://github.com/millanlaboratory/tobicore),
[xdffileio](https://github.com/millanlaboratory/xdffileio)


### Installation process
To start the installation, open a terminal and go to the installation script folder. Then type:
```shell
./install
```
The script will **automatically**:
1. Download required ubuntu packages from `apt-get`
2. If Ubuntu 18.04 or later is used, it will add specific ppa to install gcc and g++ 4.8 required by MATLAB R2017b mex compiler
3. If Ubuntu 18.04 or later is used, it will download from ubuntu website libgstreamer packages and their requirements
4. Download lab packages/libraries/modules from github or c4science
5. Donwload and install MATLABR2017b
6. Download and install gTec drivers
7. Install `Loop` packages see [Recording Loop](#Loop) for more details
10. Setup access to usb port USBamp
