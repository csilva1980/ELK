## Homework: GitHub Fundamentals and Project 13 Submission

In this assignment, you will review the concepts and procedures of git and GitHub. You will create a repository that will serve as the location where you can store any scripts, diagrams or other documentation that you have worked on throughout this course. Additionally you will be tasked with uploading the README file, network diagram, and other associated files that you have created during the ELK Stack project. Uploading these files will serve as the official submission of your project. 

Once you have completed the assignemnt, you will submit your repository link to BCS. 



### Background for ELK project

To understand GitHub, you need to know the basics of **version control**.

- Version control is a system that allows users to save all versions of a file while working on it. It's like adding an undo function to any document or file. You create save points as you work, which you can revert to at any time.

- **Git** is the most popular software used for version control. It runs on your local computer and allows you create save points (known as **commits**) for your documents. 

- You can use Git to manage any directory and track every item inside that directory. At any point, you can revert the Git directory (known as a **repository**) to a previous commit. 

GitHub is a website that allows you to sync your local Git repository with a repository in the cloud. This allows you to save your work to the cloud, share your work with others, and easily collaborate on a project. 

- Other users can access your online GitHub repository and sync their own changes. They can also make a copy of your repository to create an entirely new project based on your original project. This is known as **forking**.

In this activity, you will:

- Create a new, empty Github repository and sync it to your local machine. 

- Once your repository is up, you will add all of your Ansible scripts, Bash scripts, and network diagrams to the repository, and sync it again with the cloud. 

- When everything is synced, you will update the GitHub README file, which will explain each of the items in the repo, and display a network diagram. You will then have a GitHub repository to present to future employers. 

You will also use your GitHub account for other activities in the course.

### Required Files 

- **Ansible YAML** scripts from the Cloud Security Unit.

    - Gather all of your Ansible YAML scripts from your Ansible container on your jump box.

    - Copy and paste these into new documents on your local machine.

- **Bash scripts** from the Linux System Administration Unit.

    - Gather all of your system configuration scripts you created during the Linux weeks.

- Network diagrams from the Cloud Security and Networking Units. 

    - Gather all of the network diagrams you created during the weeks on cloud security and networking. 

### Your Goals

1. Create a GitHub repository for all of your files. 

2. Copy all of your files into the repository and create a README explaining the repository.

### Topics Covered in this Assignment

The topics covered in this homework assignment are:

- Creating a new GitHub repository.
- Syncing a local repository.
- Creating a README file.
- [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- The following commands:
    - `git pull`
    - `git add`
    - `git commit -m`
    - `git push origin --set-upstream <-branch->`

### Submission 

You will submit this assignment by submitting the link of your Github repository onto BCS. 

---

### Instructions

#### Part 1: Setting Up Your Repo 

1. Create your GitHub repository.
    - Go to [github.com](https://github.com/) and sign up for GitHub.
    - Confirm your email address.
    - Click **Create a Repository**.
    - Name your repository and give it a short description.
    - Check the box for **Initialize this repository with a README**.
    - Click **Create Repository**. 

2. Download your repository. 

    - Click the green **Clone or Download** button on the right side.
    - Copy the link.
    - Go to your command line and run the command: `git clone https://github.com/your-username/yourlink.git`
        - Enter your GitHub username and password to complete the download.


#### Part 2: Adding Files

3. Once you have the repository downloaded, copy your scripts and diagrams into it. 

    - Create folders for `Linux`, `Ansible` and `Diagrams`.

    - Copy your scripts and diagrams to the appropriate folder.

    - **Note**: Do not upload your Project files just yet. There are separate instructions for those in Part 3. 

4. Sync your local and remote repositories. 

    - In your terminal, make sure you're located in the top directory of your repo.  

    - Run `git add .` to specify that you want to sync _all_ the items and directories that you just added to your repo. This command stages your files for a commit. 

    - Run the command `git commit -m "First commit"` to confirm the commit and add a note describing it ("First commit").  

     - Run `git push` to finalize the sync.

    - Go to github.com and confirm your content is there.


#### Part 3: Adding Your Project Files

5. Add the README file and associated files that you created during Day 3 of the project week. 

    - Click on the `README.md` file in your GitHub repo.
    - Click on the small pencil that reads **Edit this file** on hover.
    - Copy and paste the `README.md` file you wrote during class. 
    - Make any desired changes and click **Commit Changes** at the bottom of the screen.

     **Note:** READMEs are written in Markdown. This [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) has more information about writing in Markdown. 



<details><summary> Instructions for creating your README.md</summary>
<br> 

The following is a duplicate of the instructions from the Day 3 README activity. If needed, refer to these instruction to complete your README. 

#### Instructions

README formats vary across projects, but you can use this template to get started: [README.zip](../Resources/README.zip).

- Download and unzip the template. Inside, you'll find a file called `README.md`, which contains the template. Much of the contents are provided, but you will need to fill in the TODO fields.

- You will also notice an `Images` folder. A few TODO items require you to place screenshots in your README. Place your screenshots in the `Images` folder, and update the README template with the appropriate file name.  

For homework, you will create a GitHub repository where you will save your project files and this README. Your repository will include:
- Your network diagram.
- A description of the deployment.
- Tables specifying access policies and network addresses.
- A description of the investigation you completed using Kibana. 
- Usage instructions.

This professional-level repository will prove you have the knowledge and communication skills that hiring managers are looking for.

While it may feel less substantial than the project itself, one of the most important skills a cybersecurity professional can have is the ability to articulate what they know. The README is an important capstone to the project and will serve as a compelling portfolio item for prospective employers.

</details>

     
<details><summary> Instructions for creating your Network Diagram</summary>
<br> 

The following is a duplicate of the instructions from the Project Week Networking Diagram activity. If needed, refer to these instruction to complete your network diagram.

#### Instructions

Use [Gliffy](https://www.gliffy.com) or [Draw.io](https://draw.io) to diagram your network. Make sure your diagram includes:

- **VNet**: Create a box that contains the machines on your virtual network. Within your VNet, diagram the following:
  - Jump box and other VMs.
  - Ansible control node.
  - Specify which VM hosts the DVWA containers.
  - Specify which VM hosts ELK stack containers.

- **Security group**: Create a box around your VNet to indicate the security group, and use a text field to specify the rules you have in place.

- **Access from the internet**: Add an icon representing the public internet and indicate how it connects to VMs in your VNet.

Use a text field to label each VM with the following information:
- Network (IP) address
- Operating system and version
- Installed containers
- Exposed ports
- Allowed IP addresses

</details>

Check your repo for any errors or typos. You now have a GitHub repository that is ready to present and share with the world. 

Once your repository is complete, submit the link on BCS. 
    
--- 
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.



Automated ELK Stack Deployment
The files in this repository were used to configure the network depicted below.
Note: The following image link needs to be updated. Diagram week 12.drawio

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the ELK file may be used to install only certain pieces of it, such as Filebeat.

TODO: ELK repository ( docker name unruffled_cartwright )

This document contains the following details:

Description of the Topologu
Access Policies
ELK Configuration

Beats in Use
Machines Being Monitored


How to Use the Ansible Build


Description of the Topology
The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.
Load balancing ensures that the application will be highly available, in addition to restricting access to the network.

TODO: What aspect of security do load balancers protect? What is the advantage of a jump box? LB protects the system from DDoS attacks by shifting attack traffic. The advantage is to give access to the user from a single node that can be secured and monitored.

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the data and system logs.

TODO: What does Filebeat watch for? Filebeat monitors the log files or locations that you specify, collects log events, and forwards them either to Elasticsearch or Logstash for indexing
TODO: What does Metricbeat record? periodically collect metrics from the operating system and from services running on the server.

The configuration details of each machine may be found below.
Note: Use the Markdown Table Generator to add/remove values from the table.

| Name    | Function   | IP address   | Operating systenm  |
|---------|------------|--------------|--------------------|
| JumpBox | gateway    | 20.85.228.13 | Ubuntu Linux 18.04 |
| web1    | VM redteam | 10.1.0.5     | Ubuntu Linux 18.04 |
| web2    | VM redteam | 10.1.0.6     | Ubuntu Linux 18.04 |
| web3    | VM redteam | 10.1.0.7     | Ubuntu Linux 18.04 |
| ELK VM  | VM Elk     | 172.16.0.4   | Ubuntu Linux 18.04 |


Access Policies
The machines on the internal network are not exposed to the public Internet.
Only the Jump Host machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:

TODO: Public address

Machines within the network can only be accessed by the Jump Host 

TODO: Which machine did you allow to access your ELK VM? What was its IP address? Jump Host 20.85.228.13

A summary of the access policies in place can be found in the table below.


| Name    | Publicly Accessible | Allowed IP Addresses  |
|---------|---------------------|-----------------------|
| JumpBox | yes / no            | 20.85.228.13 10.1.0.4 |
| web1    | no                  | 10.1.0.5              |
| web2    | no                  | 10.1.0.6              |
| web3    | no                  | 10.1.0.7              |
| ELK VM  | no                  | 172.16.0.4            |


Elk Configuration
Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because...

TODO: What is the main advantage of automating configuration with Ansible?  It allows IT administrators to automate away configuration of several VM's at once using the representation of Infrastructure as Code (IAC)

The playbook implements the following tasks:

TODO: In 3-5 bullets, explain the steps of the ELK installation play. E.g., install Docker; download image; etc.
1- Install docker container
2- Install Elastic search
3 - Install file beats and metricbeats
4 - display data on Kibana
...

The following screenshot displays the result of running docker ps after successfully configuring the ELK instance.
Note: The following image link needs to be updated. 

![image](https://user-images.githubusercontent.com/91167262/134983759-1c909e71-ab11-4913-b11b-be9f55a50dc0.png)


Target Machines & Beats
This ELK server is configured to monitor the following machines:

TODO: 172.16.0.4

We have installed the following Beats on these machines:

TODO: FileBeats and MetricBeats

These Beats allow us to collect the following information from each machine:

TODO: In 1-2 sentences, explain what kind of data each beat collects, and provide 1 example of what you expect to see. E.g., Winlogbeat collects Windows logs, which we use to track user logon events, etc.
1- Filebeats : "A lightweight shipper for forwarding and centralizing log data". It helps you keep the simple things simple by offering a lightweight way to forward and centralize logs and files ( example : Elasticsearch)
2- MetricBeats is detailed as "A Lightweight Shipper for Metrics". Collect metrics from your systems and services. From CPU to memory, Redis to NGINX, and much more, It is a lightweight way to send system and service statistics. ( example: Kibana)


Using the Playbook
In order to use the playbook, you will need to have an Ansible control node already configured. Assuming you have such a control node provisioned:
SSH into the control node and follow the steps below:

Copy the ansible config file to roles folder.
Update the config file to include VM IP addresses
Run the playbook, and navigate to Kibana to check that the installation worked as expected.

TODO: Answer the following questions to fill in the blanks:

Which file is the playbook? Where do you copy it? Ansible-Playbook - filebeat-playbook.yml ( into /etc/ansible/roles)
Which file do you update to make Ansible run the playbook on a specific machine? How do I specify which machine to install the ELK server on versus which to install Filebeat on? ansible.cfg ( by chanhging webserver VM's or elk VM enable # )
_Which URL do you navigate to in order to check that the ELK server is running? http://104.46.199.105:5601/app/kibana


