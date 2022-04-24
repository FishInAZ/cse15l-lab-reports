# Lab Report 2 week 4

## Purpose -- improve the program

These are the changes that I made to improve the program running process.
<img width="1212" alt="截屏2022-04-23 14 17 19" src="https://user-images.githubusercontent.com/103294608/164946248-0ca1bd5f-6c06-40e3-b788-327e1b881db3.png">
*Screen shots from the changes from Github*

## Links to the failure-inducing test files
In order to test the prorgram, there are four different test files created.

### **1. Test file symptom**

Attached is the problem of the test-file. In this test case, there's a bug whereas the code runs into infinite loop. Originally, the test file has one empty lines at the end of the test file, which leads the program go into the infinite loop and eventually crush. This error can be simply fixed by removing the empty line. Later, when running this file, the progam returns the expected output.
[Failure-inducingTestFile](https://github.com/FishInAZ/cse15l-lab-reports-2-testFiles/blob/main/test-file.md)

<img width="576" alt="截屏2022-04-23 15 06 25" src="https://user-images.githubusercontent.com/103294608/164947487-9a994d74-118c-47a0-ae5a-60af61c7c780.png">


### **2. Test file 3 symptom**

Attached is the problem of the test file 3. In this test, it is asking the program to return multiple links without returning the one with an incorrect format.[InsertMultipleLinks](https://github.com/FishInAZ/cse15l-lab-reports-2-testFiles/blob/main/test-file3.md)

<img width="656" alt="截屏2022-04-23 16 10 08" src="https://user-images.githubusercontent.com/103294608/164948986-e1ac83f1-86ff-4fc2-9a37-12656838587b.png">

### **3. Test file 4 symptom**

Attached is the problem of the test file 4. In this test, it is asking the program to return an image, **which is not a link!!!**. The code supposes to not to return anything.
[Image](https://github.com/FishInAZ/cse15l-lab-reports-2-testFiles/blob/main/test-file4.md)

<img width="1071" alt="截屏2022-04-23 16 13 08" src="https://user-images.githubusercontent.com/103294608/164949088-23be8257-ad52-48c2-8fdf-6bacea1741e1.png">

### **4. Test file 5 symptom**

Attached is the problem of the test file 5. In this test, I put a fake link in the file with the wrong heading. Hence, without adding more if statement to debugg the code, it wll always cause an error when running the file. If statements are needed to correct this type of error.
[fakeLink](https://github.com/FishInAZ/cse15l-lab-reports-2-testFiles/blob/main/test-file5.md)

<img width="692" alt="截屏2022-04-23 16 21 25" src="https://user-images.githubusercontent.com/103294608/164949223-61602ef4-ab06-46df-ae8a-1224820cf630.png">

## What is the relationship between the bug, the symptom, and the failure-inducing input?

While **bug** is a flaw in the program or the system, a **symptom** is a faulty program behavior programmers can see. Moreover, **failure-inducing input** enables bug to execute and symptoms to appear.

