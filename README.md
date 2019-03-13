# Lab Installation Scripts

## How to create an installation script
* Create a list of all required default ubuntu packages (e.g. cmake, git, g++)
* Check minimum version necessary for each package (use your current version)
* Install every package through a loop with `sudo apt-get install name-of-package`
* Download and install lab packages through [loop installation](https://github.com/millanlaboratory/installationScripts/tree/master/loop/install)
* Download your packages by **cloning** your github repositories
* Compile and/or install them automatically thanks to cmake, autoconf, scons or meson

## Add your script to this folder
If not already done, clone repository: 
```bash
git clone https://github.com/millanlaboratory/installationScripts
```
Once cloned, go to the repository and move your script to a new folder with the name of your project:
```bash
cd installationScripts
git pull
NAMEOFPROJECT="nameOfProject"
mkdir $NAMEOFPROJECT
cp /path/to/your/installationScript $NAMEOFPROJECT/
git add .
git commit -m "adding installation script for $NAMEOFPROJECT"
```
**IMPORTANT** Make sure to add a complete README.md about the steps you are doing in the installation. Use the template in the loop folder.

## Available installation scripts
* [Recording Loop](https://github.com/millanlaboratory/installationScripts/tree/master/loop#Loop)
* [Sinergia Project](https://github.com/millanlaboratory/installationScripts/tree/master/sinergia#Sinergia)
