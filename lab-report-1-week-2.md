# Hello! incoming 15L students

This blog will be covering the steps to set up _ieng6_ account.

Step 1: Installing [VScode](https://code.visualstudio.com/download)

<img width="927" alt="截屏2022-04-08 19 27 54" src="https://user-images.githubusercontent.com/103294608/162553314-b08a079f-a5ae-41f1-9c18-8d700bfa5ee5.png">

Step 2: Remotely Connecting

After installing VSCode. You should be able to connect to your virtual machine through a few commands.

first, you have to type in the comman "ssh <username>@ieng6.ucsd.edu"

Then, you should enter your password.
  
Upon successful login, you should be able to see the image below:
  
<img width="419" alt="截屏2022-04-08 19 38 45" src="https://user-images.githubusercontent.com/103294608/162553489-deafb21e-5c4e-40d7-bf4c-c01235e6f033.png">

  
Step 3: Trying some commands
  
There're few commands you can try on your own after logging on to the virtual machine
  
cd ~

cd

ls -lat

ls -a

ls <directory> where <directory> is
  
e.g
  
<img width="462" alt="截屏2022-04-08 19 46 18" src="https://user-images.githubusercontent.com/103294608/162553655-c5c1e8c5-33ea-43e9-ad8a-0b91be6ec02f.png">


Step 4: Moving Files with _scp_

**What is _scp_ ?**

It is to secure copy the file from the local machine to the virtual machine using ssh. However, it requires the user to enter the password everytime when processing a file. An example of this notion is attached below.
  
 <img width="95" alt="截屏2022-04-09 12 57 13" src="https://user-images.githubusercontent.com/103294608/162589755-c08719fb-98d9-4567-b4d9-809eefb4ea92.png"> then a username is required to eneter at the end.
  
  
Step 5: Setting an SSH Key
 
 Instead of entering the password everytime, setting up an SSH Key allows the user to scp files to virtual machine without the need to enter the password.
 The command _ssh-keygen_ is used to generate the password. By following the instructions pop up at the VSCode, a keygen will be automatically saved at the destination the user wants. Next time, a scp can be performed by using the command line below without enetering the password repeatedly.
  **scp /Users/<user-name>/.ssh/id_rsa.pub username@ieng6.ucsd.edu:~/.ssh/authorized_keys**
  <img width="727" alt="截屏2022-04-09 13 23 26" src="https://user-images.githubusercontent.com/103294608/162590471-df1223d2-7574-4ddc-a809-f2c6f0c98ad0.png">
  
  
Step 6: Optimizing Remote Running
  
You can now access the virtual machine with more ease with the command below.
 <img width="725" alt="截屏2022-04-09 13 34 52" src="https://user-images.githubusercontent.com/103294608/162590808-01c77971-1eeb-45ae-8e32-de84e1202468.png">

  
 Thank You!
 


