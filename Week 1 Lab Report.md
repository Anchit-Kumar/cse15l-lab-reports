# Summary
In this lab session we create a CSE 15L account, ssh into our account and try different commands.\
We also create our own github page to display our work and learn markdown in order to display text on a webpage!

# Setting Up an Account 
We first look at our course account for CSE 15L at the link: \
[course account](https://sdacs.ucsd.edu/~icc/index.php)\
and then follow the on-screen instructions to reset the password for the account.
  
# Visual Studio Code
We then need to download and set up Visual Studio Code which since I already had I didn't need to.\
You can download it at this site [VSCode Set-Up Link](https://code.visualstudio.com/) 
  
If you have a system running Windows you would also need to implement a few other steps first before you can proceed. \
The first step is installing git. You can do this from this site: \
[Download git here](https://gitforwindows.org/) 
  
Once that's done, you would need to implement the steps in the following post in order to set your default terminal \
to use the newly installed `git bash` on VSCode:
[Setting up git bash on VSCode for Windows](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) \
This is what VSCode should look like once you have it downloaded and set up: \
![Image](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-12%20at%202.23.56%20PM.png)

# Remotely Connecting
We can then remotely connect to the remote server. Since I used a mac, I opened the integrated terminal on \
VSCode first. This can be done by right clicking on a file and clicking on the option 'Open in Integrated \
Terminal'. You can also click on 'View' and then select 'Terminal' or use the keyboard shortcut 'Ctrl + \`' \
You can also perform similar steps to open the terminal on Windows or go to 'Terminal' then 'New Terminal' as well.
  
I then used the command:
`ssh cs15lwi23abc@ieng6.ucsd.edu` \
where abc is replaced by our course specific account. 
  
This is what I saw upon logging in: \
![Image](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-13%20at%205.07.24%20PM.png)
  
# Running Commands
We can then run commands on the remote server. Here are some of the commands I tried: \
![Image](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-13%20at%205.11.20%20PM.png)
This is what some of the commands seen in the image above do: \
*cd* - This command is used to change the working directory to the directory mentioned after this command \
*ls* - This command prints out all the files in the current working directory \
*ls -lat* - This command prints out all the files in the current working directory sorted by date and also with \
information about readability, writeability, executability and user. 

# Setting up Github
The aim here is to display all the work on a personalized webpage using github. \
We can do this by first setting up an account on [github](https://www.github.com) \
We then create a repository by clicking on 'Create New Repository' \
In this repository we can create a new markdown file by clicking on 'Create a new file' and naming it \
whatever we want with a .md extension. I named it Week 1 Lab Report.md \
Then to create a pages site, click on 'Settings' on the top right and then choose the 'Pages' option in \
the sidebar. Then choose 'main' as the source branch and click on 'Save'. \
It should display the message "GitHub Pages source saved" and eventually the message: \
“Your site is live at <url here>.” \
We can now view our report at the mentioned url. 
  



