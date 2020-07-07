# Offline simulation of Universal Robots and testing with Rhino-Grasshopper

![URSim Grasshopper Link](/images/01_header.png)

[URSim](https://www.universal-robots.com/download/?option=71470#section16597) is a offline simulator for Universal Robots for offline programming and simulation for robot programs and manual jogging of robots with **limited capacities**.

It also can be combined with Rhino-Grasshopper with [Robots](https://github.com/visose/Robots) to test robot codes for Universal robots _with the **limitations** mentioned earlier_. One can simulate the code, read positions, set digital outputs among many other things from Grasshopper. This project/method was very useful to test various robot codes during the recent lockdown situation without having access to a physical robot.

This method is built upon this [guide](https://academy.universal-robots.com/media/jiehhszc/ursim_vmoracle_installation_guidev03_en.pdf).

## Steps

1. Install Oracle VM Virtualbox
2. Download preferred version of URSim
3. Install URSim in VirualBox
4. Configure VMWare to connect with Windows
5. Simulate with Grasshopper

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

1. Open Oracle Vm VirtualBox Manager and click on 'New'

![Click on New](/images/03_ursim_vm_start.jpg)

2. Give it a relevant name and chose where to keep the Virual Machine. On machine type select **Linux** and Version as **Ubuntu 64 Bit**.

![Machine Type](/images/04_ursim_vm_chose_OS_type.jpg)

3. Assign around 1-2 GB of memory depending on your base system

![Assign memory](/images/05_ursim_vm_assign_ram.jpg)

4. Next step is to assign an existing hard disk. When prompted, clck on _Use and Existing virtual hard disk file_ and click on the Folder icon beside it.

![Select HD](/images/06_ursim_vm_chose_hd_1.jpg)

5. Click on _Add_ and browse to the folder where you have extracted the URSim ZIP file and select the file on top of the list.

![Select HD1](/images/06_ursim_vm_chose_hd_2.jpg)

![Select HD2](/images/06_ursim_vm_chose_hd_3.jpg)

6. Now click on _Create_ button and your Virtual Machine will be ready.

![Select HD3](/images/06_ursim_vm_chose_hd_4.jpg)

7. Now click on the settings to change a crucial network property and a display property.

![Created VM](/images/06_ursim_vm_create.jpg)

8.  On _Display_ tab change the Graphics Controller to VBoxSVGA.

![Change Display](/images/07_ursim_vm_display.jpg)

9. On _Network_ tab change the _Attached to_ to _Host-only Adapter_

![Change Network](/images/07_ursim_vm_network.jpg)

10. Now you can start your Virtual Machine.
