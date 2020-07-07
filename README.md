# Offline simulation of Universal Robots and testing with Rhino-Grasshopper

![URSim Grasshopper Link](/images/01_header.png)

[URSim](https://www.universal-robots.com/download/?option=71470#section16597) is a offline simulator for Universal Robots for offline programming and simulation for robot programs and manual jogging of robots with **limited capacities**.

It also can be combined with Rhino-Grasshopper with [Robots](https://github.com/visose/Robots) to test robot codes for Universal robots _with the **limitations** mentioned earlier_. One can simulate the code, read positions, set digital outputs among many other things from Grasshopper. This project/method was very useful to test various robot codes during the recent lockdown situation without having access to a physical robot.

This method is built upon this [guide](https://academy.universal-robots.com/media/jiehhszc/ursim_vmoracle_installation_guidev03_en.pdf).

## Steps

* Install Oracle VM Virtualbox
* Download preferred version of URSim
* Install URSim in VirualBox
* Configure VMWare to connect with Windows
* Simulate with Grasshopper

# 1. Install Oracle VirualBox

* Download Oracle VM VirualBox from [here](https://www.oracle.com/virtualization/technologies/vm/virtualbox.html) and install.

# 2. Download preferred version of URSim
* Download your preferred version of URSim ( CB-series or e-Series) from [here](https://www.universal-robots.com/download/). This guide is meant for Windows. So when prompted please chose the *non linux* version of the software. While downloading you need to follow the steps in the download link.
  * **1. Robot Type:** either CB or e Series (mine is a CB series)
  * **2. Select type of download for CB-Series:**  Software
  * **3. Select type of software:** Offline simulator
  * **4.Select operating system for your computer:** Non linux
  * **5.Select Software version:** 3.13.* (Mine is 3.13. You can chose to have older version even)
* Save the Zip file and Unzip the contents of the file to a folder with preferably administrative rights.
* The contents of the folder should look like this.

![URSim Unzipped](/images/02_ursim_unzipped.PNG)

# 3. Install Install URSim in Virtualbox
__*Now follow the steps to get a working version of URSim in VM VirualBox*__

* Open Oracle Vm VirtualBox Manager and click on 'New'

![Click on New](/images/03_ursim_vm_start.jpg)

* Give it a relevant name and chose where to keep the Virual Machine. On machine type select **Linux** and Version as **Ubuntu 64 Bit**.

![Mahcine Type](/images/04_ursim_vm_chose_OS_type.jpg)

*
