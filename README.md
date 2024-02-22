This project is designed to guide you through the basics of setting up a simple website, creating a web server, and deploying changes manually. Each phase builds upon the previous one, gradually introducing you to fundamental concepts in web development and DevOps.

Phase 1: Simple Website

To begin, we'll create a basic website on GitHub.

Create GitHub Account: Sign up on GitHub.
Create Repository: Create a repository named website on GitHub.
Clone Repository: Clone your website repository locally using your terminal (Terminal on Mac or PowerShell on Windows).
bash
Copy code
git clone <repository_url>
Create Branch: Create a branch called feature_index.
bash
Copy code
git checkout -b feature_index
Add index.html: Add a file index.html to the branch containing the text "Hello, World!". You can use Visual Studio Code for this.
Commit Changes:
bash
Copy code
git add index.html
git commit -m "Add index.html with Hello, World!"
Push Changes:
bash
Copy code
git push origin feature_index
Create Pull Request: Create a pull request for your branch to be merged into master and assign the pull request to your mentor. If you don’t have a mentor, assign it to mhedgpeth.
Merge Pull Request: Merge your pull request into master after it’s approved.
Resources for Phase 1
Try Git in 15 minutes
Getting Started with Visual Studio Code
Codecademy Learn HTML
Phase 2: Simple Webserver

Now, let's set up a server to host our website.

Create Azure Account: Create an account on Azure and activate your free trial.
Create Ubuntu Virtual Machine: Create an Ubuntu virtual machine on Azure.
SSH to the Machine: SSH to that machine. If you’re on Windows, use Matt Wrock’s guide to get an ssh client.
Set up Nginx: Set up nginx on the machine.
Clone Repository: Clone your git repository to /var/www/html on the server.
Access Website: Using the public IP assigned to your Ubuntu server, access the website (e.g., http://[your-ip]). Your website should show up.
Share with a Friend: Have a friend on another computer access the website. They should see it too.
Resources for Phase 2
Setting Up Linux Virtual Machine on Azure
Nginx Tutorial
Nano Tutorial for editing text files in an SSH session
Phase 3: Deploy a Change

Now, let's deploy a change to our website.

Update index.html: Update index.html to say "Hello, Michael!".
Create Pull Request: Create a pull request, get it reviewed, and merge it.
Update Website: On your webserver, update your index.html file from GitHub.
What We’re Learning
This phase teaches us the manual deployment process, emphasizing the importance of understanding the manual steps before automating them.
