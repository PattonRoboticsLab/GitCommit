# GitCommit

To add this function to a project, perform the following steps:
1. Navigate to a folder where you want to save the function (I saved it to my C drive. C:\Users\Username\MATLAB). In the Command Window write this line of code:  
    	**!git clone https://github.com/PattonRoboticsLab/GitCommit.git**
2. In your main code, add the following lines:  
    	**Path1 = 'path/to/current/folder';  
			Path2 = 'path/to/GitCommit/function';  
			addpath(Path1) //tells Matlab where to look for the file  
			cd(Path2)      //Navigates to GitCommit folder  
			!git pull		//Pulls any changes to that code  
			cd(Path1)		//Navigates back to main code folder**  
4. You can call the function from the Command Window or add it to the end of your code to automatically commit the changes:	
   	 **GitCommit('message')**  
  	 Change the message to whatever you want it to be.

This code checks to make sure git is installed, that there is an active local directory, and that you are connected to git with your email.

If all of these check out, then it will pull any recent changes, add all files in the staging area, commit the changes, and push to the desired branch. 
