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

`ter logining into or creating a Microsoft Azure account you will be on the home screen. In the search bar type Resource Group (RG) and click on that option to go to the Resource Group page. On this page in the top left corner click the creatre button to create a Resource Group an be taken to the create a (RG) page (refer to image 1). On the create a Resource Group page type the name of your (RG) in the tab, then select a region to save the data in (refer to image 2). Next press the review+create button (refer to image 3) and then the create button (refer to image 4) to actually have the Resource Group made.

![image](https://github.com/user-attachments/assets/8ecf164a-2440-4a74-a6e5-7b3def1f659d)
<p>Image 1
</p>

![image](https://github.com/user-attachments/assets/01838b92-b0e2-4f62-b11d-a4d30f1d9c5a)
<p>Image 2
</p>

![image](https://github.com/user-attachments/assets/a49416d7-6bdb-4f56-bce0-f765f35de347)
<p>Image 3
</p>

![image](https://github.com/user-attachments/assets/4658e411-7320-4460-b52d-30efefb3aa88)
<p>Image 4
</p>

Next you create the Virtual Network. In the search bar type Virtual Network (VN) and click that option to go to the VN's home page. On the home page in the top left corner click the create button to go to the Create a Virtual Network page (refer to image 5). On this page type the name of you (VN), and place the Virtual Network under the previously made Resource Group and in the same region as the resource group (refer to image 6). Next click the review+create button and then the create buttton.

![image](https://github.com/user-attachments/assets/2ba22787-26cb-48ed-866b-38b8d36c8f2f)
<p>Image 5
</p>

![image](https://github.com/user-attachments/assets/a63ef035-f213-4c96-8100-0aa29ace084f)

<p>Image 6
</p>

Next we create the two Virtual Machines, for demonstration purposes "Dc-1" and "Client-1". Dc-1 is going to be a server while Client-1 is going to be a Windows operating Virtual Machine (VM). To create a (VM) first go to the search bar and type Virtual Machines and click on that option to go the the (VM) home page. On this home page in the top left corner click create and choose "Azure Virtual Machine" option from the drop down menu to go to the create a (VM) page (refer to image 7). On create a virtual machine page name it "DC-1", then place it in same region and resource group, next set security type to standard, pick the "Windows Server 2022" image (refer to image 8). Secondly set the user name and password, and check the license box, then click the disk tab at the bottom (refer to image 9). Next click the network tab (refer to image 10) and on the networking sub page make sure the (VM) is put in the Virtual Network created in previous steps (refer to image 11). Lastly press review+create (refer to image 12) and then create (refer to image 13).

![image](https://github.com/user-attachments/assets/c25ee35e-f0e8-4bc2-bd2b-3c060223b336)
<p>Image 7
</p>

![image](https://github.com/user-attachments/assets/fbb1f3c1-da0a-4e45-8888-cf60cc66ddb0)
<p>Image 8
</p>

![image](https://github.com/user-attachments/assets/b1bb605b-ca39-4f8b-9058-25cd1a491f8c)
<p>Image 9
</p>

![image](https://github.com/user-attachments/assets/617fcfb8-0f56-43c3-8625-02197298af42)
<p>Image 10
</p>

![image](https://github.com/user-attachments/assets/409804be-1833-4b0e-9349-b76e91098b05)
<p>Image 11
</p>

![image](https://github.com/user-attachments/assets/ba43c57b-885f-4ac7-a240-415cbb77a9b8)
<p>Image 12
</p>

![image](https://github.com/user-attachments/assets/fbf282c3-0a51-46ef-9ef4-52c13c33cf9c)
<p>Image 13
</p>


Now create "Client-1" Virtual Machine. To create a (VM) first go to the search bar and type Virtual Machines and click on that option to go the the (VM) home page. On this home page in the top left corner click create and choose "Azure Virtual Machine" option from the drop down menu to go to the create a (VM) page (refer to image 14). On create a virtual machine page name it "Client-1", then place it in same region and resource group, next set security type to standard, pick the "Windows 10 Pro, versi0n 22H2" image (refer to image 15). Secondly set the user name and password, and check the license box, then click the disk tab at the bottom (refer to image 16). Next click the network tab (refer to image 17) and on the networking sub page make sure the (VM) is put in the Virtual Network created in previous steps (refer to image 18). Lastly press review+create (refer to image 19) and then create (refer to image 20).

![image](https://github.com/user-attachments/assets/c25ee35e-f0e8-4bc2-bd2b-3c060223b336)
<p>Image 14
</p>

![image](https://github.com/user-attachments/assets/70bef57e-05ea-4060-af75-585dd2752b81)
<p>Image 15
</p>

![image](https://github.com/user-attachments/assets/00de40b2-97f2-465b-9c83-48f1e6e790da)
<p>Image 16
</p>

![image](https://github.com/user-attachments/assets/da8a5033-f132-466a-a8b1-7fe85d613c85)
<p>Image 17
</p>

![image](https://github.com/user-attachments/assets/f97a9803-c6e5-4bfd-8181-159d5d1ef35f)
<p>Image 18
</p>

![image](https://github.com/user-attachments/assets/c207c679-838c-40b4-9630-7acf98040629)
<p>Image 19
</p>

![image](https://github.com/user-attachments/assets/aa35a7f7-76fa-4d6e-8da7-d0cda847e8cd)
<p>Image 20
</p>



