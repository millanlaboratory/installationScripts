## <span id="Sinergia"> Sinergia </span>
**OS tested:** Ubuntu 14.04 LTS & 16.04 LTS (laptop & desktop), Ubuntu 18.04 LTS & 19.04 (desktop only)

**Duration:** ~1h30min if MATLAB is not already installed. 15min otherwise.

**After installation these packages will be installed:**
cmake,
[cnbitkextra](https://github.com/millanlaboratory/cnbitkextra),
[cnbitkloop](https://github.com/millanlaboratory/cnbitkloop),
[cnbi-smrtrain](https://github.com/millanlaboratory/cnbi-smrtrain),
[drawtk](https://github.com/millanlaboratory/drawtk),
[eegc](https://github.com/millanlaboratory/eegc),
[eegdev](https://github.com/millanlaboratory/eegdev),
[eegview](https://github.com/millanlaboratory/eegview),
[fescontrol](https://github.com/millanlaboratory/fescontrol),
[fesinit](https://github.com/millanlaboratory/fesinit),
libcanberra-gtk-module,
libjsoncpp-dev,
libsdl-mixer1.2-dev,
[lpttrigger](https://github.com/millanlaboratory/lpttrigger),
[mcpanel](https://github.com/millanlaboratory/mcpanel),
meson,
[patient-alloc](https://github.com/millanlaboratory/patient-alloc),
python3,
python3-pip,
python-pip,
python-matplotlib,
python-numpy,
python2.7-dev,
python3-tk,
[rtfilter](https://github.com/millanlaboratory/rtfilter),
[tobicore](https://github.com/millanlaboratory/tobicore),
[xdffileio](https://github.com/millanlaboratory/xdffileio)

### Installation process
To start the installation, open a terminal and go to the installation script folder. Then type:
```shell
./installSinergiaPackages
```
The script will **automatically**:
1. Download required ubuntu packages from `apt-get`
2. If Ubuntu 18.04 or later is used, it will add specific ppa to install gcc and g++ 4.8 required by MATLAB R2017b mex compiler
3. If Ubuntu 18.04 or later is used, it will download from ubuntu website libgstreamer packages and their requirements
4. Download lab packages/libraries/modules from github or c4science
5. Donwload and install MATLABR2017b
6. Download and install gTec drivers
7. Install `Loop` packages see [Recording Loop](https://github.com/millanlaboratory/installationScripts/tree/master/loop#Loop) for more details
8. Install `FESControl` module and its library libjsoncpp
9. Install `Patient-Allocator`
10. Setup access to usb port for FES and USBamp
11. Create Desktop shortcuts for FESInit, Launcher, FES Movement testers (Sensory, Flexion & Extension), Machine learning and Patient allocation
12. Add SSH Key to list to allow connection of the Patient Allocator to the database
It will install desktop shortcuts to facilitate the use of the system for physiotherapists. In order to connect to the database properly, it will also add ssh key.

**Warning** When `patient-alloc` is connecting to the database for the first time, it will ask to allow this host in the terminal. Type `yes` and press enter to accept.

![Sinergia Project Diagram should be here](https://raw.githubusercontent.com/millanlaboratory/installationScripts/master/sinergia/SinergiaDiagram.png "Sinergia project diagram")
