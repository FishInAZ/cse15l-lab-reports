# Lab Report 5 Week 10

### How to find tests with different results?

I used `vimdiff` to find the difference between the file's result.

### Below are the links to the test files I usedfor this Lab Report

1. [Test File 194](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)
2. [Test File 481](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/481.md)

# Test File 194
The expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="1166" alt="截屏2022-06-05 20 24 27" src="https://user-images.githubusercontent.com/103294608/172089367-a4250864-1dd7-496a-a363-fa718e068436.png">

After running the command `vimdiff`, I obtain the following results 

<img width="1350" alt="截屏2022-06-05 21 23 59" src="https://user-images.githubusercontent.com/103294608/172094587-f9206cc9-b879-4988-ba26-5f41ed8e5f5b.png">

*On the left, it is the output obtained by my own markdown parse; on the right, it is the output obtained by the given codes*

### Which implementation is correct?

Both implementation obtained the wrong results based on the expected output produced by the link provided in the write-up.

### Bug

The bug of the given program is that the code returns a wrong link when it should've return something different. This outcome may be caused by brand new form of giving a link. Conventionally, a link is given by the form `[]()`. However, in this case, the link is given in the form of `:`. In the given code, the program recognizes only `()`, so it will automatically think that `[url]` is the result we want to obtain. In my code, on the other hand, it also recognizes the same format, which is `[]()`. Hence, it also return the same result as the given code, while giving more output.

*Given code*

<img width="559" alt="截屏2022-06-05 21 51 15" src="https://user-images.githubusercontent.com/103294608/172096941-06a21ed8-9a55-44e2-91c6-8d4c4f138199.png">

*My code*

<img width="514" alt="截屏2022-06-05 21 56 22" src="https://user-images.githubusercontent.com/103294608/172097410-a2f6793c-d2e7-44be-b782-2520423c6b69.png">


# Test File 481

The expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="1158" alt="截屏2022-06-05 22 01 06" src="https://user-images.githubusercontent.com/103294608/172098035-8f5f178f-6548-46e4-bafa-533bd959cd6e.png">

After running the command `vimdiff`, I obtain the following results

<img width="1382" alt="截屏2022-06-05 22 02 22" src="https://user-images.githubusercontent.com/103294608/172097914-af9c9490-c73a-475f-96b6-28a41ca2918b.png">

*On the left, it is the output obtained by my own markdown parse; on the right, it is the output obtained by the given codes*

### Which implementation is correct?

My code, in this case, is correct. However, the given code is obtaning a wrong output.

### Bug

The bug of the given program is that the code returns a wrong link when it should've return something different. This outcome may be caused by this part of the program

<img width="464" alt="截屏2022-06-05 22 24 34" src="https://user-images.githubusercontent.com/103294608/172100036-1160aa5b-cc29-4b20-9cc0-372707e8a5e2.png">

The program thinks, the logic of the given link is wrong, so it automatically returns an empty Array List, hence, causing the error.


