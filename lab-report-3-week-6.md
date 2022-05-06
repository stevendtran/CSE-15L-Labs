# Lab Report 3

## Streamlining ssh Configuration
1. I was using a windows machine so I manually went into the .ssh file in the user to make the config file. Then I copied and pasted the user and hostname into the config file.  
![Picture](PicLab3/config.png)
2. With that I no longer had to type in the hostname and username instead I used the alias ieng6.  
![Picture](PicLab3/alias.png)
3. I used the `scp` command to copy a file from my local desktop to the ieng6 server.  
![Picture](PicLab3/scp1file.png)  
![Picture](PicLab3/filelocation.png)

## Setup Github Access from ieng6
1. The public is stored in Github in the settings.  
![Picture](PicLab3/SSHKey.png)
2. The private is store in `~/.ssh`.  
![Picture](PicLab3/privatekey.png)
3. Now you can run: `git add .`, `git commit -m ""`, and `git push` in the ieng6 terminal.  
![Picture](PicLab3/git.png)
4. Here is the [link](https://github.com/stevendtran/markdown-parse/commit/e5a0f9e5aace39f345da0c18df4d1eac1663aed7) to that commit.  

## Copy whole directories with scp -r
1. Copying over the whole markdown-parse directory into ieng6 account.
![Picture](PicLab3/copy.png)
2. Here I will be running the tester in markdown-parse using `javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java` and `java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest`.  
![Picture](PicLab3/runningtest.png)  
3. Combining `scp` and `ssh` using `;` to copy the whole directory and run all the test in one line.  
![Picture](PicLab3/combine1.png)  
![Picture](PicLab3/combine2.png)  

P.S. My lab group an I were unable to solve one of the testers, so in the pictures only 8/9 of the test pass.
