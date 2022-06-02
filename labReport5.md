# Week 10 - Lab Report 5

I was able to find the test with the differenet results using vimdiff. By typing in `vimdiff markdown-parser/results.txt NewMarkdown/results.txt` the terminals shows the reults of the test and highlights those that are different.  
![Picture](PicLab5/vimdiff.png)  

[Test file with different result #1](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)    
This is the result of the given code:
![Picture](PicLab5/givencode194.png)  
This is the result of my code:
![Picture](PicLab5/mycode194.png)  

For this my implementation of code is correct and gives the correct output, an empty arraylist. While the given code output was incorrect. The arraylist is empty because there is no link in the test file so, nothing can be put into the arraylist. As seen in the preview of the test file 194, the text is not linked to a link.  
![Picture](PicLab5/pre194.png)  

[Test file with different result #2](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)    
This is the result of the given code:
![Picture](PicLab5/givencode201.png)  
This is the result of my code:
![Picture](PicLab5/mycode201.png)  

For this test file given code was correct a returned with a arraylist containing one link. However, my code returned an empty arraylist. When looking at the preview for test file 201 we can see that the text is linked to a link.  
![Picture](PicLab5/pre201.png)

### Fixes
