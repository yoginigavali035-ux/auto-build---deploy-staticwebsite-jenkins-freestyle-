# auto-build---deploy-staticwebsite-jenkins-freestyle-

📌 Project Overview

This project demonstrates a basic Jenkins Freestyle job that automatically pulls code from a GitHub repository and deploys a simple static website to a server folder. It shows basic CI/CD automation using Jenkins and Git.

# 🛠 Tools Used

GitHub

AWS EC2 (Ubuntu)

Jenkins

Git

# Linux commands

📂 Project Steps
# Step 1 — Create GitHub Repository

Created a new GitHub repository

Added a simple index.html file

Pushed the code to GitHub

![image alt](https://github.com/yoginigavali035-ux/auto-build---deploy-staticwebsite-jenkins-freestyle-/blob/main/images/create%20repository.png)


# Step 2 — Launch EC2 Instance

Launched Ubuntu EC2 instance

Configured Security Group

Opened required ports:

8080 → Jenkins

80 → Web access (optional)

# Step 3 — Install Jenkins

Connected to server using PowerShell (SSH)

Installed Java

Installed Jenkins

Started Jenkins service

Accessed Jenkins using:

http://54.251.131.78:8080

# Step 4 — Initial Jenkins Setup

Unlocked Jenkins

Completed initial setup

Installed suggested plugins

# Step 5 — Install Required Plugins

Installed plugins:

Git plugin

GitHub integration plugin

# Step 6 — Create Jenkins Freestyle Job

Created new Freestyle project

Connected GitHub repository URL

Configured Source Code Management → Git

# Step 7 — Configure Build Step

Added Execute Shell build step:

sudo mkdir -p /home/ubuntu/deploy
sudo cp -r * /home/ubuntu/deploy/


This command copies project files from Jenkins workspace to deploy folder.

# Step 8 — Build Trigger Setup

Enabled Poll SCM or GitHub Webhook

Automation triggers build when code changes are pushed

# ✅ Result

Jenkins successfully pulls code from GitHub

Build runs automatically

Files are deployed to server directory

Basic CI automation achieved

# 🎯 Learning Outcome

Jenkins installation and setup

Freestyle job creation

GitHub integration

Build triggers (Poll SCM / Webhook)

Basic deployment using shell commands
