# Lab Report 4
--

1. `ssh cs15lwi23agw@ieng6.ucsd.edu` Log in into ieng6 server. It doesn't require password because I configure the ssh key to my local machine
<img width="512" alt="image" src="https://user-images.githubusercontent.com/68884486/221387523-f285f33a-b2d7-4b63-b58e-ffbcd918c24d.png">

2. `git clone git@github.com:ericljx2020-gmail/lab7.git`clone the forked repository to home directory of ieng6 server. Since we have set up the ssh key, we can use ssh git clone so that later when we push the changes to github, we don't have to enter the password and username. 
<img width="406" alt="image" src="https://user-images.githubusercontent.com/68884486/221387689-26f701c5-bee5-4912-b7a6-f21c9989ccfe.png">
above is the place where we copy the ssh clone address in the forked repository.
<img width="598" alt="image" src="https://user-images.githubusercontent.com/68884486/221387786-ff7ef8e3-0645-400f-a623-8286be7c314a.png">

3. `ls` we see that there is a directory named "lab7". 
<img width="683" alt="image" src="https://user-images.githubusercontent.com/68884486/221387835-2801d1c7-d93d-4154-8bf9-3102a514ba58.png">

4. `cd lab7` so that we get into lab7 directory
5. `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` to compile all java files in lab7 
6. `ls` to see that there are classes of these java files
<img width="758" alt="image" src="https://user-images.githubusercontent.com/68884486/221387949-10ba0dcb-5d88-47bd-b52f-d46fb307e8b8.png">
7. `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` to run the ListexampleTests and the result is shown below. There is bugs so that I should try to fix it.
<img width="975" alt="image" src="https://user-images.githubusercontent.com/68884486/221387992-c1d01152-9b65-4153-bf2c-b2667c5ec420.png">
8. `vim ListExamples.java` so that we can edit the java file.
<img width="599" alt="image" src="https://user-images.githubusercontent.com/68884486/221388050-9e63a792-c27b-4460-af83-d84e128572f0.png">
9. we find the bug is that when comparing 2, the index that should be updated is index2 instead of index1 which I have shown the change in the picture.
<img width="614" alt="image" src="https://user-images.githubusercontent.com/68884486/221388104-beacd4c7-45f6-4aee-8819-ab13902af8a2.png">
After changing the buggy code, type `ESC -> :wq -> ENTER` to save and quit file
10. `up up up` to compile the java files again.
11.  `up up up` to run the tests again now it passes the test
<img width="978" alt="image" src="https://user-images.githubusercontent.com/68884486/221388208-a4da6f27-8942-4612-9c64-1f98c9ef43c5.png">
12. `git add *` add all files in lab7 directory to be ready to commit
13. `git commit -m "fix bug"` save changes to files that added
<img width="526" alt="image" src="https://user-images.githubusercontent.com/68884486/221388282-8dfd4aa9-d4ef-45ba-999f-8f73dedf98a0.png">
15. `git push` push the changes to the github repository below image shows that chanegs are successfully committed.
<img width="534" alt="image" src="https://user-images.githubusercontent.com/68884486/221388288-c487f73a-9f39-4759-8be5-256f889c3786.png">
<img width="1308" alt="image" src="https://user-images.githubusercontent.com/68884486/221388344-ea7f66b3-c666-434e-94fb-6100a447ffc7.png">
This page on github shows that commit has been successfully saved

This is all we have for this lab
