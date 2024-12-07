# Preparing Active Directory Environment Within Microsoft Azure Virtual Machine Part2
![image](https://github.com/user-attachments/assets/e4f41676-9505-49cf-82a1-c1ad2d5cf390)



This is part 2 of an outline of the steps needed to be completed before installing Active Directory. In this project protion we will be adjust the two virtual networks created in part one.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Virtual Machines: DC-1, Client-1
- Internet 

<h2>List of Prerequisites</h2>

- Laptop or Desktop Pc                                                                                                                                 
- Wifi Access
- Microsoft Azure Account
- Previously created Virtual Machines

<h2>Procedure Steps</h2>

First Dc-1's needs to be configured that the server remains the same preventing the ip address from changing, and prevent the firewall from blocking Client-1's traffic or access to the server.
<p>
</p>
On the account home screen uderneath the recent activity screen click the "DC-1" virtual machine name to be take to it's home page. In the left corner of "DC-1's" home page has menu options, click the networking option and select network settings from the drop down to gain access the virtual Network Interface Card (nic) . Click on the card the be able to configure it's settings. At the middle of the page you will see "ipconfig1", click on it to be able to edit the ip address settings. In the right corner of the screen in the "Edit Ip configuration" screen, change the allocation from dynamic to static, then save the setting  by clicking save at the bottom.


Next you have to turn off the server firewalls. This is done by firstly using Remote Desktop the connect wth "DC-1" server. Open Remote Desktop and type DC-1's public ip address that you can get from DC-1's home page, next type the username and password created in part 1 of this project. After logging in the bottom left corner in the search bar type "Run" and open the app. In the run app type "wf.msc" to open Windows defender firewall. In the middle of the window is the hyperlink "Windows Defender Firewall Properties," click on it to be able to change it's settings. In the settings window under the sub windows Domain, Private, and Public Profile in the firewall state change all of them from on to off. Lastly click Apply and then Ok at the bottom before closing the window.

