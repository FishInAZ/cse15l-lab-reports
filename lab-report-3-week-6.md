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

<img width="1032" alt="截屏2022-05-09 13 33 41" src="https://user-images.githubusercontent.com/103294608/167493068-0a914fa7-1538-4d49-85a1-a990fc989c61.png">


### Step 3
I then use a serious of `git` commands to push a new file to my ieng6 account.

<img width="529" alt="截屏2022-05-07 22 26 05" src="https://user-images.githubusercontent.com/103294608/167283157-10304e6d-2768-49fc-8613-4aca0c5104ab.png">

### Step 4
This is the [link](https://github.com/FishInAZ/cse15l-lab-reports) to my commit shown above.

## 3. Copy whole directories with `scp -r`

### Step 1

By using the command `scp -r . ieng6:~/makrdown-parse`, I copy the entire directory to my ieng6 account as shown:

<img width="1349" alt="截屏2022-05-09 13 41 38" src="https://user-images.githubusercontent.com/103294608/167494248-85b45dfb-c31c-447e-9e8c-089a4fc55caf.png">

<img width="1346" alt="截屏2022-05-09 13 41 59" src="https://user-images.githubusercontent.com/103294608/167494301-ea98e0cf-6837-48e1-961f-4cdaea2d4f1e.png">

### Step 2

After logging onto my ieng6 specific account, I use the command `ls` and find the file `markdown-parse` I just uploaded in the previous step.

<img width="881" alt="截屏2022-05-09 13 42 51" src="https://user-images.githubusercontent.com/103294608/167494438-5df714c9-7f9a-4829-9618-bb6105e30737.png">

Then, I use the command `cd markdown-parse` to open the file I upload. With the two command lines `javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java` and `java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest`, I was able to run the JUnit test.

<img width="1035" alt="截屏2022-05-09 13 47 02" src="https://user-images.githubusercontent.com/103294608/167495666-c67b7685-10f0-4a0c-903b-83299e9c3f36.png">

<img width="1035" alt="截屏2022-05-09 13 51 32" src="https://user-images.githubusercontent.com/103294608/167496349-81a1811d-4f5c-4d25-aac0-e561b7de1696.png">

### Step 3

In order to use the shorter commands to do the same thing as above, I use the following command:

`scp -r *.java *.md lib/ ieng6:markdown-parse; ssh ieng6 "cd markdown-parse; javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`;

Essentially, I just put everything I had previously in one command line, and seperate them by using `;`.

<img width="1387" alt="截屏2022-05-09 13 57 42" src="https://user-images.githubusercontent.com/103294608/167497387-e61a00c2-21fe-41f7-bd3c-b5ef5f74afd3.png">
