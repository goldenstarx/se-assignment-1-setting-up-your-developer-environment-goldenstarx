Developer Environment Setup Documentation

## TABLE OF CONTENT

1. Windows 11 Installation
2. IDE Instalation
3. Version Control System Setup
4. Programing Languages and Routines Installation
5. Package Managers Insatallation
6. Database Installation and Configuration
7. Development Environments and Virtualization Setup
8. Code Editor Extentions Installation

### Introduction
This document offers a thorough walkthrough for configuring, installing, and troubleshooting common problems while setting up a developer environment.

### 1. Select your Operating System 

**Prefered OS:** Windows 11 (Already installed)

### 2. IDE Installation

**Text Editor/IDE:** Visual Studio Code

**Steps to Install Visual Studio Code:**

1. **Download Visual Studio Code**
- Go to Visual Studio Code Download page.
- Click on the "Windows" button to download the installer.

2. **Install Visual Studio Code**
- After the download is complete, locate the installer file in your Downloads folder.
- Double-click the installer file to run it.
- Follow the setup wizard:
  - Click "Next" to continue.
  - Accept the license agreement and click "Next".
  - Choose the destination folder and click "Next".
  - Select additional tasks (like creating a desktop icon) and click "Next".
  - Click "Install" to start the installation.
  - Once installation is complete, click "Finish" to launch Visual Studio Code.

### 3. Version Control System Setup

**Version Control System:** Git

**Steps to Install Git:**

1. **Install Git**
- Go to Git for Windows.
- Download the installer and run it.
- Follow the setup instructions, selecting the default options unless specific preferences are needed.

2. **Configure Git**
- Open Git Bash (installed with Git).
- Set your username and email:
  - git config --global user.name "Your Name"
  - git config --global user.email "your.email@example.com"

3. **Create Git Hub Account**
- Go to GitHub and sign up for a new account.

4. **Instalize a Git Repository**
- Open a terminal or Git Bash.
- Navigate to your project directory or create a new on:
  - mkdir my_project
  - cd my_project
- Initialize the Git repository:
  - git init
- Create a sample file and make your first commit:
  - echo "# My Project" >> README.md
  - git add README.md
  - git commit -m "Initial commit"

5. **Push to GitHub**
- Create a new repository on GitHub.
- Follow the instructions provided to push your local repository to GitHub:
  - git remote add origin https://github.com/yourusername/your-repo.git
  - git branch -M main
  - git push -u origin main

### 4.  Programing Languages and Routines Installation

**Programming Language:** Python

**Steps to Install Python**

1. **Download and Install Phyton**
- Go to Python's official website.
- Download the latest version for Windows.
- Run the installer and ensure "Add Python to PATH" is checked.
- Follow the installation steps.

2. **Verify Installation:**
- Open a terminal or command prompt.
- Verify Python installation:
  - python --version
- Install pip (if not included):
  - python -m ensurepip --upgrade

### 5. Package Managers Insatallation

**Package Manager:** pip for (Phyton)

**Steps to Install pip**

1. **Verify pip Installation**
- Open a terminal or command prompt.
- Verify pip installation:
  - pip --version

2. **Upgrade pip**
- Upgrade pip to the latest version:
  - python -m pip install --upgrade pip

### 6. Database Installation and Configuration

**Configure a Database:** MySQL

**Steps to Install MySQL**

1. **Download MySQL**
- Go to MySQL Community Downloads.
- Download the MySQL Installer.

2. **Install MySQL**
- Run the MySQL Installer.
- Choose "Custom" setup type for more control.
- Select the MySQL Server and other components as needed.
- Follow the installation steps.
- Configure MySQL Server:
  - Set the root password.
  - Configure MySQL as a Windows Service.
- Complete the installation.

3. **Verify Installation**
- Open MySQL Workbench or a terminal.
- Connect to the MySQL server using the root account.

### 7. Development Environments and Virtualization Setup

**Optional Tools:** Docket or Virtual Machines

**Steps to Install Docker**

1. **Install Docker**
- Go to Docker Desktop.
- Download Docker Desktop for Windows.
- Run the installer and follow the instructions.
- Verify installation:
  - docker --version

2. **Create a Dockerfile for your Project**
- In your project directory, create a 'Dockerfile' to define your environment.

3. **Build and Run Your Docker Container**
- Build your Docker image:
  - docker build -t my_project_image .
- Run your Docker container:
  - docker run -d -p 8000:8000 my_project_image

### 8. Code Editor Extentions Installation

**Explore Extentions and Plugins**

**Extentions and Plugins for Visual Studio Code**

**Steps to Install Extentions and Plugins**

1. **Install Extentions**
- Open Visual Studio Code.
- Click on the Extensions icon in the Activity Bar.
- Search for and install relevant extensions (e.g., Python, GitLens, Prettier, ESLint).

2. **Configure Extentions**
- Configure extensions as needed through the settings or configuration files (e.g., .'prettierrc', .'eslintrc'.json').



**Reflection of The Challenges faced During Setup and Strategies Employed to Overcome Them**

I ran into a few difficulties throughout the setup process, like PATH configurations that prevented the MySQL server from starting properly. I had to change environment variables and reinstall MySQL with the proper settings in order to fix issues. These encounters brought to light the significance of paying close attention to installation instructions and the requirement for troubleshooting abilities when establishing a development environment.
