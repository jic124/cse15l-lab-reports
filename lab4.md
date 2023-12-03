# Lab Report 4 - Vim

* **Log into ieng6**
  ![image](lab4_1.png) <br>
  ```ssh cs15lfa23qq@ieng6.ucsd.edu```
  
* **Clone your fork of the repository from your Github account (using the SSH URL)**
  ![image](lab4_2.png) <br>
  ```git clone git@github.com:jic124/lab7.git```

* **Run the tests, demonstrating that they fail**
  ![image](lab4_3.png) <br>
  ```ls``` and ```cd``` commands, as shown in the screenshots, were used to move to the directory ```lab7```.
  Then, ```bash test.sh``` to run the tests.
  
* **Edit the code file to fix the failing test**
  ```vim ListExamples.java```
  ![image](lab4_4.png) <br>
  pressed keys: ```14+j+<enter>+e+r+2+:+w+q+<enter>``` <br>
  ```14j``` skips 14 lines. ```<enter>``` skips an additional line - in total 15 lines skipped.
  ```e``` moves the cursor to the end of the word, and ```r2``` replaces the letter under the cursor to ```2``` - 1 to 2.
  Finally, ```:wq<enter>``` saves the file and exits vim.
  
  ![image](lab4_5.png)

* **Run the tests, demonstrating that they now succeed**
  ![image](lab4_6.png) <br>
  ```bash test.sh``` to rerun the tests. 
  
* **Commit and push the resulting change to your Github account**
  ![image](lab4_7.png) <br>
  ```git add .``` adds all the changes made to the staging area. ```git commit -m "yay"``` records the changes in the ```main branch``` with the message ```yay```, and ```git push origin main``` updates the local changes to the remote repository. 
