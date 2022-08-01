# GIT-with-SSH

<img width="541" alt="git with ssh" src="https://user-images.githubusercontent.com/110182832/182138969-e7f19ad4-5793-474c-9e03-ccd3da1f095b.png">



## How to create repository in GITHUB and push/pull the file using ssh from GITBASH
## Follow these steps

- Create a new repository on github account ( In this case we will create a repo without README.md file and we will create README.md file in our system and then push it to the github)

- We will create a directory/ folder in the local host with the same name as repository name to avoid any confusion
-Now, Open terminal(gitbash) as an admin
- Make sure that you are not in master/main/.ssh folder
- <img width="230" alt="master" src="https://user-images.githubusercontent.com/110182832/182131299-d81eb1a4-79a2-4f6e-ba14-1bf62dae4628.png">

- If you're in master/main or .ssh folder as shown above then you need to get out of that folder by entering following commands.
- cd(space) enter
- If you're still in master/main folder then enter following command

- rm -rf .git 
- Now, you'll be out of master/main folder

- Now, create a directory in the localhost/system with the same name as repository name. ( In this case we are using eng122_week2 for both repository name and the name of directory in the system)
- mkdir eng122_week2
- Now go into that directory by
- cd eng122_week2

- Now you should be in that directory/folder that you just created 

<img width="250" alt="cd" src="https://user-images.githubusercontent.com/110182832/182132303-686c3410-3584-43a9-a98f-18bac7a11fe0.png">
- To check this run 
pwd 
- It will show the location of your current directory like
- /c/users/bhadr/eng122_week2

- Now, if you run
 ls -a
 - There should be no files in that dir, it will show you ./ ../
 
 - Now create a file into that directory using 
   nano README.md
 - You'll enter into nano editor, edit your file and to save press ctrl + x , then exit the editor and press Y.
 
 - Now, follow the steps shown in to git accout 
 
 - Initialise the file by
   git init 
 - Now to check enter 
   ls -a or ls ( it will show the list of files in that directory )
   
   <img width="310" alt="ls" src="https://user-images.githubusercontent.com/110182832/182133507-ce46bce9-12ca-44ae-81c2-b9bf0e841371.png">

- Now run 
- git add file name 
- git add README.md
- git status (the name of file should appear green)
- git commit -m"message"
- git branch -M main   
- git remote add origin git@github.com:ArpitB95/eng122_week2.git ( You can copy this code from the steps shown in your git account)
- git push -u origin main

- Now go back to your git account and refresh it, you will find the file README.md in eng122_week2 repository

- After pushing the file if it shows an below error 

 <img width="288" alt="error" src="https://user-images.githubusercontent.com/110182832/182134577-071496df-1e8b-4c0e-88a0-d85af5671f2d.png">

- Then enter this command and push again
- eval "$(ssh-agent -s)"
- ssh-add ~/.ssh/122
- git push -u origin main

- Now refresh the git account page and the file will be there.


