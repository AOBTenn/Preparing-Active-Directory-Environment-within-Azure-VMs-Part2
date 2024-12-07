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
On the account home screen uderneath the recent activity screen click the "DC-1" virtual machine name to be take to it's home page. In the left corner of "DC-1's" home page has menu options, click the networking option and select network settings from the drop down to gain access the virtual Network Interface Card (nic) . Click on the card the be able to configure it's settings. At the middle of the page you will see "ipconfig1", click on it to be able to edit the ip address settings. In the right corner of the screen in the "Edit Ip configuration" screen, change the allocation from dynamic to static, then save the setting by clicking save at the bottom.

![image](https://github.com/user-attachments/assets/7eb4dcf8-8ffc-4136-a95a-c98148a6832a)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/21fa6642-f1d3-480d-affa-cbe592c51bd6)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/e96c9b3a-6a53-4fb7-bc8d-d4e510c3a847)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/88e1d076-7f11-48f7-831d-3f342199cd67)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/bb30ac61-f532-4f04-b749-33b4ce666984)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/16121a5d-9295-4017-8a72-5f3b5d59396e)



Next you have to turn off the server firewalls. This is done by firstly using Remote Desktop the connect wth "DC-1" server. Open Remote Desktop and type DC-1's public ip address that you can get from DC-1's home page, next type the username and password created in part 1 of this project. After logging in the bottom left corner in the search bar type "Run" and open the app. In the run app type "wf.msc" to open Windows defender firewall. In the middle of the window is the hyperlink "Windows Defender Firewall Properties," click on it to be able to change it's settings. In the settings window under the sub windows Domain, Private, and Public Profile in the firewall state change all of them from on to off. Lastly click Apply and then Ok at the bottom before closing the window.


![image](https://github.com/user-attachments/assets/9ac13ad0-fd9f-454e-af8c-c8e791bc46e2)
![image](https://github.com/user-attachments/assets/cfaeddd9-9db6-4a54-b129-884bc1c96f7f)
![image](https://github.com/user-attachments/assets/6f520bc1-b1be-49e5-ad48-9f1fd051df89)
![image](https://github.com/user-attachments/assets/56c8987b-6f61-4eaa-90f8-536b9b8a06cb)
![image](https://github.com/user-attachments/assets/636cb1d7-e2d5-43bb-b875-598f5e458811)
![image](https://github.com/user-attachments/assets/a7a5f790-dc4a-45ca-8d66-8fef150746c5)
![image](https://github.com/user-attachments/assets/998f8829-67f0-4f88-91aa-6aa6c0633b13)



(refer to image 1)
