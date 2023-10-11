Andrew Bodzsar & Team - 09.2020

This project was completed by a team of 4 members for the Advanced Algorithms & Data Structures module of the Computer Security and Forensics course, at the University of Greenwich. It implements Dijkstra's algorithm to find the shortest route between two given underground stations, which can be manually selected. Journey times have been manually assigned to each station, therefore a total time is displayed on the results page.

*** README: please follow the below instructions to run our London Underground Journey Planner ***

Prerequisites - make sure you have the following installed on your development machine:

1. Python => 3.7
2. pip
3. Virtualenv - this can be downloaded using the following command: 'pip install virtualenv' 

Package Requirements (must be installed within your virtual environment, discussed below in instruction 1):

* Django==3.1.3
* django-crispy-forms==1.9.2
* openpyxl==3.0.5
* pandas==1.1.4
* xlrd==1.2.0


Project Installation:

1. Set up a local development environment (venv) in the current directory (where this file is located). A venv can be created in the following way:
	open PowerShell and navigate to this directory and enter the following command: 'virtualenv .' or 'py -m venv env', if the first command does not work.
	Lib and Scripts folders should now have been created in your current directory as confirmation of the successful venv setup. ***See below if this has not worked correctly
2. Now run your venv using the following command: "./Scripts/Activate" or "env/Scripts/Activate", and install the above package requirements (the current versions must be called explicity)
3. Once you have installed the above packages, change directories to 'src/LondonUndergroundPlanner' - this folder should contain the manage.py file.
4. Prior to running your local server, please copy 'home_page.html' and 'results_page.html' from 'src/LondonUndergroundPlanner/templates' and paste them into the following
	directory: 'LondonUndergroundPlanner\Lib\site-packages\django\contrib\admin\templates' - this is done so that Django knows where to find the correct html files to render.
5. To run the web application locally enter the following command: 'python manage.py runserver'	
6. This will run the local server and return your local address (127.0.0.1:8000). Enter this into a browser (Chrome preferred) and the program should now run successfully.

*** If the venv has not been created successfully, make sure that your Powershell settings are updated: 
	1. Open Powershell in administration mode, confirm security pop-up if required
	2. Enter: Set-ExecutionPolicy Unrestricted, and select y/yes (this means you should only have to do this once)
	3. Now close this terminal, reopen Powershell (admin mode is not required at this point) and go back over step 1 above.



Other Important Points:

* To access all files it is recommended to open the src/LondonUndergroundPlanner folder within an IDE (VisualStudio recommended) in order to view the full hierarchical structure of Django
* All relevant coursework code can be found in the course_work code folder within our Django Project. All other files and folders allow us to run Django correctly however, you may also be interested in the following files:

	1a. views.py - file handles coursework functionality by taking user input, running all algorithms and then rendering this to the user.
	1b. forms.py - file handles our form class used to take input from the user on page one.
	1c. static - contains photos and css style sheets.	
	1d. templates - contains html files rendered to the user 

* To deactivate your virtual environment enter 'deactivate' at your command prompt.
