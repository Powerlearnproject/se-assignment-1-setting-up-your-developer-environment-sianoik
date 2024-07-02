[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15269721&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11/ 
   Operating system: Linux Ubuntu 22.04 LTS
   Requirements: 2GHz dual-core processor
                 4gb ram
                 25 gb of free hard drive space
Installing linux ubuntu on a laptop involves several steps. STEP 1
    - Backup your data: ensure that you back up any important documents since installation erases everything. check that the system is compatible with mininmum requirements. 
                   STEP 2
                   Download Ubuntu ISO https://ubuntu.com/download/desktop 
Create a bootable USB, download Etcher and install, Open etcher and download the Ubuntu ISO file, select the USB drive, click 'flash' to create bootable USB
   STEP 3: Boot from USB Drive
   - insert USB to your laptop, restart your laptop and enter BIOS settings, change boot order, save and edit
   STEP 4: INSTALL UBUNTU
   -Choose "Try Ubuntu": When the Ubuntu boot menu appears, select "Try Ubuntu" to load the live session.
   -Start the Installer: In the live session, double-click the "Install Ubuntu" icon on the desktop to start the installation process.
   -Select Language: Choose your preferred language and click "Continue".
   -Keyboard Layout: Select your keyboard layout and click "Continue".
   -Updates and Other Software: Choose whether to install updates and third-party software for graphics and Wi-Fi hardware and additional media formats. Click "Continue".
   -Erase Disk and Install Ubuntu: This option will delete all data on the disk and install Ubuntu.
   -Allocate Drive Space: If you chose "Erase Disk and Install Ubuntu", select the disk you want to use and click "Install Now". Confirm any warnings about data loss.
   -Time Zone: Select your time zone and click "Continue".
   -User Information: Enter your name, a computer name, a username, and a password. Click "Continue".

   STEP 5: 
   -wait for installation to complete
   -Restart the pc once the intallation is complete 
   -Log in using the password and user name created. 

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download 
    Installing Vscode for linux
    - https://code.visualstudio.com/docs/setup/linux
    1. update the system: sudo apt update
    2. Install dependencies: sudo apt install software-properties-common apt-transport-https wget
    3. enable vscode repository:sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
    4. install vscode: sudo apt install code
    5. launch Vs code



3. Set Up Version  System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com 
   https://github.com/sianoik  - created github account 
   steps of creating a github account;
   - visit the website for github https://github.com/
   - on homepage; click sign up
   -  enter account details such as username, and email address, set up the password
   - complete the verification process
   - set up profile such as profile picture, bio and important links
   - start using your github 


4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.

  installing python: python on linux is pre-installed python3 -v
  write a simple python programme print("Hello, World!")


5. Install Package Managers:
   If applicable, install package managers like pip (Python).
   check pip install: pip3 --version this will show the type of pip installed
   - to install sudo apt update
sudo apt install python3-pip


6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
   https://dev.mysql.com/downloads/mysql/ using the link to the website download mysql and follow procedural 
   to connect mysql with python:
   import mysql.connector. 
from mysql.connector import Error

try:
    connection = mysql.connector.connect(
        host='localhost',
        database='mydatabase',
        user='myuser',
        password='mypassword'
    )
    if connection.is_connected():
        db_Info = connection.get_server_info()
        print("Connected to MySQL Server version ", db_Info)
        cursor = connection.cursor()
        cursor.execute("select database();")
        record = cursor.fetchone()
        print("You're connected to database: ", record)

except Error as e:
    print("Error while connecting to MySQL", e)
finally:
    if connection.is_connected():
        cursor.close()
        connection.close()
        print("MySQL connection is closed")


7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
 Docker: 