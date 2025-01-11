<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Network Security Groups(NSGs) and Inspecting Network Protocols!</h1>
In this tutorial we are going to be doing some excercises involving looking into the DNS Cache, pinging to a host server, nslookup and ipconfig in Powershell!<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Highlights</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>A-Record Excercise</h2>

<p>
We are going to be using our "DC-1" and "Client-1" VMs again for this lab! If you have not yet created them, go to my other lab for Active Directory Configuration https://github.com/michaelxflow/Active-Directory-Config
<p>
</p>

<img src="https://github.com/user-attachments/assets/cc5c1bce-dbd5-4838-937c-0cd5201688d9" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First let log into "Client-1" as an admin "mydomain.com\jim_admin" and password "Password123!"
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/042dec02-4410-473c-9e70-00acdf05d837" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Log in to "DC-1" as your admin as well!
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/797ecda2-23bc-4975-92c5-07b3aac596ba" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From Client-1 open up powershell in the search bar, we are going to then try to ping to DC-1 host mainframe name!
</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/06d2a4ac-3577-4fcd-859a-a7773a65934f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type "ping mainframe" in Powershell and it will try to locate the host. We have not configured it yet in DC-1 so it cannot locate it. The computer will run in powershell to check its "Local DNS Cache". If nothings found it will check the "Local Host File". If that has also failed it will lastly check the "DNS Server". It is fastest to check the cache first bacause it is temporaly installed memory thats easy to pull up for the computer.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6e25ff79-d8a4-45c3-a1f8-a5bfb9117a0c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You can also type "ipconfig /displaydns" and it will show a list of the cache in the dns. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b6ef650d-708c-4659-8474-3e356985ce49" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/0781278d-5241-40bd-9721-780880b3962a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6e4fbc73-d059-4823-bbc2-6dfa061c078f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/fde5558b-b2d5-4b7f-857b-211b23850864" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/c6b56cfb-006e-49d4-9353-550fad7efac2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2d235b80-946b-4223-9145-d545f021ad37" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9118362a-f2bf-43c6-8942-17fd427197eb" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/2b3f75c5-598c-46c8-95bc-800a8eb449be" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7409dee7-ae53-498b-8afd-754a13ddd1c3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e957fd27-dc6b-4ceb-8b5f-1c14bec7df35" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<h2>Local DNS Cache Excercises</h2>


<p>
<img src="https://github.com/user-attachments/assets/4371d04f-059f-47cb-a708-da9f22c06607" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2400e815-f6d2-4003-8789-22f9623aee97" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7b70947b-0709-4922-99bc-7a4bade88637" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<img src="https://github.com/user-attachments/assets/f45699f8-d770-467c-acc7-85aa5dc88bc0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/2c0d2817-61d6-4932-b9ac-498b7d7ca6d9" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<h2>Create a CNAME Record</h2>



<p>
<img src="https://github.com/user-attachments/assets/54745603-fff3-48ff-ac6d-5e4509164660" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/fffa0deb-791f-4c5f-8d0d-84ab2699d060" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/436777f5-2a28-43b2-aae0-9993dc00406f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<h2>End of Lab!</h2>

</P>
<p>
Now we are finished with a few of these excercises! I hope you learned some new things today! There is many more to learn!
<p>
</p>
