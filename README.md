# Home Assistant on Windows  
### Installing and setting up Home Assistant OS on Windows using virtual machine software  
<br/>
  
***Overview :***  <br/>
Let's learn how to install Home Assistant OS on a Windows platform using virtual machine software (ex. [Oracle VM Virtual Box](https://www.virtualbox.org/)) and getting started with the basics.  
<br/>    
  
### Home Assistant  
<br/>
  
There are many cloud based IoT dashboard providers that can allow you to control your IoT devices. There are restrictions that are associated with each provider, and scaling these platforms requires us to pay them for their services. But did you ever wondwer if we could use our own hardware and setup soemthing like a cloud server that could connect various devices? *[Home Assistant](https://www.home-assistant.io/)* is the open-source software that makes this possible. This repository provides you with the exact things that you need to get started with Home Assistant.  
<br/>  

***Supported Devices:***  
Home Assistant OS is supported on various devices. some of which are:  
- Raspberry Pi
- Asus Tinker Board
- Mac OS, Linux and Windows (Virtualization Software)  
 <br/> 
  
### Installing Oracle VM Virtual Box  
Head over to the official download site for Virtual Box ([here](https://www.virtualbox.org/wiki/Downloads)) and download the platform package for Windows. Next, launch the intaller and follow the on-screen instructions to install the Virtual Box on Windows.  
<br/>  
  
### Installing Home Assistant on Virtual Box  
Follow the below steps to install Home Assistant OS on Virtual box.  
- Download the `.vdi` file for virtual box from [here](https://www.home-assistant.io/installation/windows).
- Once downloaded, open the Virtual Box software and click on `New` button.
- Select a suitable name, and install directory. 
- In the type drop-down list, select `Linux`, and in the Version, select `Linux 2.6/3.x/4.x (64bit)`. Click on next.
- Assign atleast 2GB RAM. Check the `Enable EFI (special OSes only)` check box. Click on next.
- In the next window, select `Use an existing Virtual disk` and select the previously downloaded `.vdi` file. Select next.
- Once the VM is created, head over to VM settings. Under the `Network Adapter` section, choose `Bridged Adapter`. Select the network adapter that you are using.
  
That's it for installing Home Assistant on Virtual box.  
<br/>  
  
### Initial Setup in Home Assistant Web UI  
Once installation is done, launch the VM, and wait for it to boot up successfully. Once done, Home Assistant OS should show you an IP address and a link using which the Web UI can be accessed. It takes some time for the Web UI to configure. Once over, proceed to creating a user and login. Save the username and password in a safe place, as they are needed to login into your account on any device.  
  
On any other device that is connected to the same WiFi as your Windows PC, just use the IP address to open the Home Assistant Web UI. Link format - `http://<IP Address>:8123` replace the IP address with address provided on Home Assistant VM. You can use the same link to link with your Home Assistant Companion app on [Android](https://play.google.com/store/apps/details?id=io.homeassistant.companion.android&hl=en_IN&gl=US) and [iOS](https://apps.apple.com/us/app/home-assistant/id1099568401) too.  
<br/>  
  
***And That's It!***  
You've successfully installed Home Assistant OS on your Virtual Box. But that's not it, check out my other repositories to find out on how to install [Mosquitto MQTT Broker](https://github.com/Bharadwaj-R/Mosquitto-MQTT-on-Home-Assistant) and [Node-RED](https://github.com/Bharadwaj-R/Node-RED-and-Home-Assistant) on Home Assistant to get started with MQTT over Home Assistant.
