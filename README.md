# Sysmon-Install

In this repository I will be doing a walk through of how to install sysmon on a Windows virtual machine.

In this setup I will be running a Windows 10 Virtual machine on Vmware. The iso file for this machine can be downloaded from the following link:

https://info.microsoft.com/ww-landing-windows-10-enterprise.html

After the virtual machine is set up we want to open a browser and navigate to the following link:

learn.microsoft.com/en-us/sysinternals/downloads/sysmon

You should see this screen when you open up the link


<img width="718" alt="Sysmon Landing Page" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/30d9263d-0f48-453b-afd5-31714e5a373b">

Select the option "Download Sysmon", if you wish to download it for a Linux machine then select the option below that one.

While that is downloading go ahead and also download the sysmon configuration file found at this link:

github.com/olafhartong/sysmon-modular/blob/master/sysmonconfig.xml

This link will bring you to the following Github page


<img width="935" alt="Sysmon Configuration File" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/50b630c1-5687-4dc3-96a4-d7ce427759b0">

Click on the RAW button

Right-click within the file and select save as, this will save the file to the downloads folder

The sysmon install file should be downloaded by now so go ahead and navigate to the downloads folder within windows and locate the zip file named sysmon. 

Right-click and select Extract Files


<img width="512" alt="Extract Option for Sysmon" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/90b925d2-ebc8-4e69-8217-9ebc2d752931">


Do not click the executable, instead we are going to want to open a Powershell window, select "Run as Administrator"


<img width="514" alt="Windows Powershell" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/2663b388-c336-4a6e-991e-806850af6580">

Once in the command prompt we want to make sure we are in the same directory as the sysmon file that we juat extracted, to do this we will want to highlight the file path.












