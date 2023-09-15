# Sysmon-Install

In this repository I will be doing a walk through of how to install sysmon on a Windows virtual machine.





For my setup I will be running a Windows 10 Virtual machine on Vmware. The iso file for this machine can be downloaded from the following link:

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

Once in the command prompt we want to make sure we are in the same directory as the sysmon file that we juat extracted, to do this we will want to copy the file path.


![image](https://github.com/MustangGuy86/sysmon-install/assets/103835436/99a5a7ae-be76-4f91-9139-5f9586f68d1e)


Paste this into Powershell and append the cd command to the beginning, please note that your path may differ from mine since we will have different machine names.


<img width="515" alt="Sysmon Directory Path" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/b774dbac-e3f2-4409-81b4-9f99b2bab394">

We then want to make sure that our sysmon configuration file is within the same directory, this can be done by simply dragging the sysmon.config file within downloads and dropping it into the extracted sysmon file which is also within Downloads.

Now type in the command .\Sysmon64.exe and hit enter, this will bring up the help options for this command.

We want to now install sysmon with the configuration file, the command to do so should look like the following.


<img width="374" alt="sysmon config command" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/7369f63f-ede2-4df3-980a-93c8805a382f">

When you run this command a dialogue box will pop up for the licensing agreement just select AGREE and the installation will commence.

Once the installation is complete we can verify that sysmon has successfully installed in one of two ways:


1.  Type services in the search bar on the desktop. Once in Services scroll down until you see Sysmon64


   
<img width="406" alt="Sysmon 64" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/0445166c-b345-4461-a700-34d58f6bdb28">

   


2. Type Services within the search bar on the desktop, on the left pane select Applications and Services --> Microsoft --> Windows --> Scroll down untill you see Sysmon.


<img width="445" alt="Event Viewer Sysmon" src="https://github.com/MustangGuy86/sysmon-install/assets/103835436/8fa9c1a3-fad3-436e-8d63-11ad4075ab7a">


Sysmon has now successfully been installed.





