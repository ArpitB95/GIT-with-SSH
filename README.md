# GIT-with-SSH


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
   


