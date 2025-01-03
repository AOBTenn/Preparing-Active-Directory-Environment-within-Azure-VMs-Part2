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
On Microsoft Azure account home screen uderneath the recent activity screen click the DC-1 virtual machine name to be take to it's home page (refer to image 1 and 2). In the left corner of DC-1's home page has menu options, click the networking option and select network settings from the drop down to gain access the virtual Network Interface Card (nic) (refer to image 3) . Click on the (nic) to be able to configure it's settings. At the middle of the page you will see "ipconfig1" (refer to image 4), click on it to be able to edit the ip address settings. In the right corner of the screen in the "Edit Ip configuration" screen, change the allocation from dynamic to static, then save the setting by clicking save at the bottom (refer to image 5 and 6).

![image](https://github.com/user-attachments/assets/7eb4dcf8-8ffc-4136-a95a-c98148a6832a)
<p>Image 1
</p>

![image](https://github.com/user-attachments/assets/21fa6642-f1d3-480d-affa-cbe592c51bd6)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/e96c9b3a-6a53-4fb7-bc8d-d4e510c3a847)
<p>Image 3
</p>

![image](https://github.com/user-attachments/assets/88e1d076-7f11-48f7-831d-3f342199cd67)
<p>Image 4
</p>

![image](https://github.com/user-attachments/assets/bb30ac61-f532-4f04-b749-33b4ce666984)
<p>Image 5
</p>

![image](https://github.com/user-attachments/assets/16121a5d-9295-4017-8a72-5f3b5d59396e)
<p>Image 6
</p>


Next you have to turn off the server firewalls. This is done by firstly using Remote Desktop the connect wth DC-1 server. Open Remote Desktop and type DC-1's public ip address that you can get from DC-1's home page (refer to image 7 and 8), next type the username and password created in part 1 of this project (refer to image 9). After logging in the bottom left corner in the search bar type "Run" and open the app (refer to image 10). In the run app type "wf.msc" to open Windows defender firewall (refer to image 11). In the middle of the window is the hyperlink "Windows Defender Firewall Properties," click on it to be able to change it's settings (refer to image 12). In the settings window under the sub windows Domain, Private, and Public Profile in the firewall state change all of them from on to off (refer to image 13). Lastly click Apply and then Ok at the bottom before closing the window.


![image](https://github.com/user-attachments/assets/9ac13ad0-fd9f-454e-af8c-c8e791bc46e2)
<p>Image 7
</p>

![image](https://github.com/user-attachments/assets/cfaeddd9-9db6-4a54-b129-884bc1c96f7f)
<p>Image 8
</p>

![image](https://github.com/user-attachments/assets/6f520bc1-b1be-49e5-ad48-9f1fd051df89)
<p>Image 9
</p>

![image](https://github.com/user-attachments/assets/56c8987b-6f61-4eaa-90f8-536b9b8a06cb)
<p>Image 10
</p>

![image](https://github.com/user-attachments/assets/636cb1d7-e2d5-43bb-b875-598f5e458811)
<p>Image 11
</p>

![image](https://github.com/user-attachments/assets/a7a5f790-dc4a-45ca-8d66-8fef150746c5)
<p>Image 12
</p>

![image](https://github.com/user-attachments/assets/998f8829-67f0-4f88-91aa-6aa6c0633b13)
<p>Image 13
</p>
<p>
</p>
Now we must configure Client-1's ip address for it to use DC-1 server as the Domain Controller within Microsoft Azure for the purpose of this project. This is easily done by setting Client-1's private ip address to that of DC-1's private ip address.
<p>
</p>
The first step is to go back to DC1's home screen, and in the middle of the home page you wil find the private ip address, copy it to a notepad or write it down to use later (refer to image 14). Next go back to Microsoft Azure account home screen uderneath the recent activity screen click the Client-1 virtual machine name to be take to it's home page (refer to image 15 and 16). In the left corner of Client-1's home page has menu options, click the networking option and select network settings (refer to image 17) from the drop down to gain access the virtual Network Interface Card (nic). Click on the (nic) to be able to access it's settings (refer to image 18). Under the settings you wil see "DNS servers" option (refer to image 19), click on it to customize it. In this DNS server page click on "Custom" (refer to image 20). Under Custom type Dc-1's private ip address and then click save. Lastly go back to Client-1's hone page and reset The virtual machine for the change to take effect (refer to image 21). 


![image](https://github.com/user-attachments/assets/9fcb6431-cfe4-46cd-b635-a6fd7d88c31b)
<p>Image 14
</p>

![image](https://github.com/user-attachments/assets/7f64e20f-8cea-4c45-9d7a-b1cd25f7846a)
<p>Image 15
</p>

![image](https://github.com/user-attachments/assets/234e4879-98f3-4b4c-9fd0-7840fa9c7abe)
<p>Image 16
</p>

![image](https://github.com/user-attachments/assets/e803beb6-325b-4721-9e2f-86f9c1676396)
<p>Image 17
</p>

![image](https://github.com/user-attachments/assets/711711bd-310b-40f5-9c8a-8a180d002fe7)
<p>Image 18
</p>

![image](https://github.com/user-attachments/assets/e9aa5e23-6c74-4ffb-9337-2c5da41b924c)
<p>Image 19
</p>

![image](https://github.com/user-attachments/assets/4f157ce6-40c7-43a9-95ba-ec0a8b5ac634)
<p>Image 20
</p>

![image](https://github.com/user-attachments/assets/56ab2e2e-ec72-41ae-a028-3d1d685ed50e)
<p>Image 21
</p>




