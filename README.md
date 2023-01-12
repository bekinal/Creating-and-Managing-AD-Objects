<h1>Creating and Managing AD Objects</h1>

<h2>Description</h2>
Project consists of using Active Directory tools to add users and create groups within a domain. 
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>Windows Server 2016</b>
- <b>Windows 10</b>

<h2>Environments Used </h2>

- <b>Windows Server 2016</b>

<h2>Users and Groups:</h2>

Open the Domain Controller (DC), and select "Tools" then "Active Directory Users and Computers": <br/>
<img src="https://i.imgur.com/eM3rYaD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right-click cyber.local. Click New, and select Organizational Unit (OU): <br/>
<img src="https://i.imgur.com/ZGLFsxY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter Sales for the name of the OU: <br/>
<img src="https://i.imgur.com/PAfTisw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click cyber.local again and note the newly created OU. Then, right click and select New, User: <br/>
<img src="https://imagizer.imageshack.com/img922/7767/bKl9T9.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the information for Salesperson1 and select Next: <br/>
<img src="https://i.imgur.com/fPyRDXu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter a password and uncheck the box "User must change password at next logon". Click next: <br/>
<img src="https://i.imgur.com/nuOS5Mx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select Finish: <br/>
<img src="https://imagizer.imageshack.com/img924/2015/mvkRR2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Repeat the steps to create users "Salesperson2" and "Salesperson3". Verify that the users were created in the Sales OU: <br/>
<img src="https://i.imgur.com/h8Atkqw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right click the Sales OU, select New, then Group: <br/>
<img src="https://i.imgur.com/7gzJQ2P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter "Sales-GRP" for the group's name: <br/>
<img src="https://i.imgur.com/XOSWyl0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right-click the group and open the Properties menu: <br/>
<img src="https://i.imgur.com/13hs6ab.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the Members tab and click Add: <br/>
<img src="https://i.imgur.com/UDKlKrs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Type Sales in the object name field and click Check Names: <br/>
<img src="https://i.imgur.com/SanOZYc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select all three users and click OK: <br/>
<img src="https://i.imgur.com/Z8MjKMW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Verify that all users were selected and click OK: <br/>
<img src="https://i.imgur.com/ycoUQgE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click Apply and OK: <br/>
<img src="https://i.imgur.com/D5bOIH7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a new user account named "Sales-Template" in the Sales OU. Right click the Sales-Template user account and select properties: <br/>
<img src="https://imagizer.imageshack.com/img924/307/ETbFpL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to the Organization tab: <br/>
<img src="https://imagizer.imageshack.com/img922/3785/fJ7UCM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the following information; Department - Sales; Company - cyber.local: <br/>
<img src="https://imagizer.imageshack.com/img922/1559/3cjLD5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to the Account tab. Click Logon Hours, select Sunday, check Logon Denied, and click OK: <br/>
<img src="https://imagizer.imageshack.com/img923/9163/bxDDu9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sundays have been restricted from the user: <br/>
<img src="https://imagizer.imageshack.com/img923/7718/zcO4Lj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Go to the Member Of tab, click Add, type Sales-GRP, click Check Names, and click OK: <br/>
<img src="https://imagizer.imageshack.com/img922/8688/7omoUY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The Sales-GRP is selected when the name is underlined: <br/>
<img src="https://imagizer.imageshack.com/img924/9180/RHiB5T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click Apply and OK to save and exit: <br/>
<img src="https://imagizer.imageshack.com/img924/5506/sConmX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right click the Sales-Template, select copy, create a new user, and name it "Salesperson4": <br/>
<img src="https://imagizer.imageshack.com/img923/8065/SXrGOF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right-click Salesperson4, choose properties. : <br/>
<img src="https://imagizer.imageshack.com/img924/9555/OtUfBo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Verify that each tab is as configured in previous steps: <br/>
<img src="https://imagizer.imageshack.com/img923/9742/D6Qd9o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to Member Of to see the Domain Users and Sales-GRP: <br/>
<img src="https://imagizer.imageshack.com/img924/3831/tpsbEn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
