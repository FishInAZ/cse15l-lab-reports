# Lab Report 4 Week 8

## This is the link -- [Markdown-parse-own](https://github.com/FishInAZ/makrdown-parse-own.git) -- to my own Markdown parse repositary.



After I run the three snippets on my own files, the results are following:

### 1. Snippet 1
For snippet 1, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="569" alt="截屏2022-05-22 13 32 31" src="https://user-images.githubusercontent.com/103294608/169714682-fe847d23-bbfe-47bc-ad5e-5a790c369f98.png">

This is the test case I wrote for snippet 1:

My code passed the test.

<img width="760" alt="截屏2022-05-22 13 49 57" src="https://user-images.githubusercontent.com/103294608/169715262-c64a0c59-04f5-4c2d-94d2-e054bcc390b2.png">


### 2. Snippet 2
For snippet 2, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="185" alt="截屏2022-05-22 13 53 25" src="https://user-images.githubusercontent.com/103294608/169715364-79b48aa9-d8fa-4029-bbc1-96c9136dbc0c.png">

This is the test case I wrote for snippet 2:

My code did not pass the test. the test failure is shown below

<img width="781" alt="截屏2022-05-22 13 55 55" src="https://user-images.githubusercontent.com/103294608/169715442-6139ae3b-904c-4e4e-bc74-a3dbff945e6d.png">


### 3. Snippet 3
For snippet 3, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="574" alt="截屏2022-05-22 13 59 20" src="https://user-images.githubusercontent.com/103294608/169715564-cea5b3cd-8c3f-4579-9d33-a39ad5b502a7.png">

This is the test case I wrote for snippet 3:

My code did not pass the test. The test failure is shown below

<img width="1274" alt="截屏2022-05-22 14 02 54" src="https://user-images.githubusercontent.com/103294608/169715680-a263ea5b-d215-45ab-8b03-741c05240048.png">


## Below is the link -- [Markdown-parse-review](https://github.com/Pgerardocastaneda/markdown-parser) -- to the repositary I reviewed on Week 7:

After I run the three snippets on my reviewed files, the results are following:

### 1. Snippet 1
For snippet 1, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="569" alt="截屏2022-05-22 13 32 31" src="https://user-images.githubusercontent.com/103294608/169714682-fe847d23-bbfe-47bc-ad5e-5a790c369f98.png">

This is the test case I wrote for snippet 1:

The reviewed code passed the test.

<img width="780" alt="截屏2022-05-22 14 09 04" src="https://user-images.githubusercontent.com/103294608/169715915-60c5bc1d-3dd4-4dcc-b5d7-d522d7e22e79.png">

### 2. Snippet 2
For snippet 2, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="185" alt="截屏2022-05-22 13 53 25" src="https://user-images.githubusercontent.com/103294608/169715364-79b48aa9-d8fa-4029-bbc1-96c9136dbc0c.png">

This is the test case I wrote for snippet 2:

The reviewed code has not passed the test.

<img width="1273" alt="截屏2022-05-22 14 10 01" src="https://user-images.githubusercontent.com/103294608/169715954-899b9b36-bb57-4c3b-8efa-22afce3d84db.png">

### 3. Snippet 3
For snippet 3, the expected output produced by [the CommonMark demo site](https://spec.commonmark.org/dingus/) is

<img width="574" alt="截屏2022-05-22 13 59 20" src="https://user-images.githubusercontent.com/103294608/169715564-cea5b3cd-8c3f-4579-9d33-a39ad5b502a7.png">

This is the test case I wrote for snippet 3:

The reviewed code has not passed the test.

<img width="1268" alt="截屏2022-05-22 14 11 04" src="https://user-images.githubusercontent.com/103294608/169715993-8ecb290c-f8da-474b-9e52-4bfcf751cb4f.png">

## Questions

### 1. Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

Both codes pass the test case for snippet 1 successfully. I think we don't necessarily have to change any code for snippet 1. It is working perfectly fine. Moreover, snippet 1 also has a relatively easier code to process comparing to the two other snippets.

### 2. Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

I think in order to address the problem in snippet 2. I have to add some lines of code to enable the code continue to process after it finds a closing parenthesis. Becuase in the case of snippet 2, it is a case where there's multiple closing parenthesis, but we only want the code to stop running after the last closing parenthesis is processed, whereas, now, my code stops running right after the first parenthesis,


### 3. Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

I can't think of a working code right now to fix the error being thrown at my snippet 3. This is because the feedback is saying that it's out of memory. Hence, I think there's more work to do to fix this kind of compiling error, instead of fixing an easy error -- the code just processed a wrong output.

