# Lab Report 3 Week 6

## 1. Streamlining ssh Configuration

### Step 1

I am creating a new file `.ssh/config` on my local machine. by using `vim ~/.ssh/config`;

### Step 2

I then edit the file as the following:

<img width="235" alt="WechatIMG590" src="https://user-images.githubusercontent.com/103294608/167282411-1d97cc40-79de-461d-b918-3c6dab76c2fd.png">

### Step 3

I then log on to my virtual machine by using the command `ssh ieng6`

<img width="482" alt="截屏2022-05-07 21 55 19" src="https://user-images.githubusercontent.com/103294608/167282424-68b5c33d-0f68-4855-baa5-0bc6febac7a4.png">

In order to enter this editing page, I first enter `I`, then I exit the page by pressing the key `esc` and the command `: wq`.

### Step 4

I then use the command `scp` to move a file from my local machine successfully to my virtual machine using the alias I chose.

<img width="936" alt="截屏2022-05-07 21 58 55" src="https://user-images.githubusercontent.com/103294608/167282502-9dd16891-5660-42d9-82c3-378417dd28ad.png">


## 2. Setup Github Access from ieng6

### Step 1

First, I created a public ssh key on my GitHub by follwoing the tutorial on [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

<img width="1307" alt="截屏2022-05-07 22 09 51" src="https://user-images.githubusercontent.com/103294608/167282760-76c83059-5b7f-4e5d-ad06-61564d2dacad.png">

### Step 2

The private Key I used is located under `.ssh/id_rsa.pub`

<img width="295" alt="截屏2022-05-07 22 15 20" src="https://user-images.githubusercontent.com/103294608/167282865-e4bc3590-63ed-40d0-9d35-4f5325e43679.png">

### Step 3
I then use a serious of `git` commands to push a new file to my ieng6 account.

<img width="529" alt="截屏2022-05-07 22 26 05" src="https://user-images.githubusercontent.com/103294608/167283157-10304e6d-2768-49fc-8613-4aca0c5104ab.png">

### Step 4
This is the [link](https://github.com/FishInAZ/cse15l-lab-reports) to my commit shown above.

## 3. Copy whole directories with `scp -r`

### Step 1

By using the command `scp -r . cs15lsp22akv@ieng6.ucsd.edu:~/cse15l-lab-reports-2-testFiles`, I copy the entire directory to my ieng6 account as shown:

<img width="1673" alt="截屏2022-05-07 22 34 43" src="https://user-images.githubusercontent.com/103294608/167283329-78d4d3ab-183a-4c70-a03e-f515d2d609a6.png">
<img width="1680" alt="截屏2022-05-07 22 35 19" src="https://user-images.githubusercontent.com/103294608/167283349-9f5dbd31-1ea5-4e7b-ac13-45b64eca5647.png">

**Note: I have my file name differently from the instruction, because of the names in my repo. I am just using this name to diffrentiate the files
I edited and the file my partner and I did in class.**

### Step 2

After logging onto my ieng6 specific account, I ran the test for the file I uploaded.

<img width="1240" alt="截屏2022-05-07 22 40 30" src="https://user-images.githubusercontent.com/103294608/167283489-844031c5-a67d-463b-a068-d572cdfd6f7e.png">

### Step 3

In order to use the shorter commands to do the same thing as above, I use the following command:

<img width="1680" alt="截屏2022-05-07 22 43 38" src="https://user-images.githubusercontent.com/103294608/167283552-753bb284-27f1-47f4-9646-8c47028d9497.png">

