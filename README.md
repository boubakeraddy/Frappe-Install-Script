
# Frappe-Bench Installation: The Saga of an Impatient Developer

Struggling with Frappe-Bench installations on different servers was a headache. Each attempt ended in frustration, forcing me to start from scratch. But giving up wasn't an option. So, I channeled my frustration into action. Determined to ease the process, I crafted a script to automate the installation. As a developer, I believed in making life easier for others. So, I turned my struggle into a solution, ensuring that no one else would face the same challenges.

---

# [Guide] How to install Frappe-bench on Linux Ubuntu (step-by-step instructions)
PRE-REQUISITES:
Operating System: Linux Ubuntu 22.04 LTS
Minimum Recommended Hardware: 2 CPU | 4 GB RAM | 20 GB Disk
Root shell access to the server (via SSH)

## To use the script for installing Frappe-Bench, follow these simple steps:
1. Pull the Script : Clone or download the script from its repository using Git or download it directly from the repository's webpage.

Repo Link = [Link text Here](https://github.com/ankittiwari2001/Frappe-Install_Script)
For Cloning it :
```bash
git clone https://github.com/ankittiwari2001/Frappe-Install_Script
```
2. Make the Script Executable:
```bash
chmod +x frappe-setup.sh
```
4. Run the Script: 
```bash
./frappe-setup.sh
```
6. Follow the Prompts: The script will prompt you for various inputs such as the Frappe version, directory name for Frappe Bench, MySQL root password, site name, etc. Follow the prompts and provide the required information.

7. Sit Back and Relax: Once you've provided all the necessary inputs, the script will take care of the rest. It will install all the required packages, configure MySQL server, set up Node.js, NPM, and Yarn, install Frappe Bench, and initialize it according to your inputs.

8. Verify Installation: After the script completes its execution, you can verify the installation by navigating to the directory where Frappe Bench was installed and checking that everything is set up correctly. 
For starting the app : got to inside app or dir by `cd <bench_dir>` and run command `bench start` .

9. Access Your Site: After the script completes the installation, you can access your site by opening a web browser and entering the site name you provided during the setup process followed by the port number 8000. For example, if your site name is demo.site.com, you would access it at demo.site.com:8000.
10. Update Hosts File: To ensure smooth access to your site, add an entry to your hosts file. Open the hosts file located at /etc/hosts using a text editor with root privileges or sudo nano /etc/hosts. Add a line with 127.0.0.1 followed by a space and then the site name you provided during the setup. Save the file and close the text editor. This step ensures that your computer knows to route requests for the site name to your local machine. For example:
```
127.0.0.1   demo.site.com
```

This is my first code blog, so I apologize in advance if there are any errors.
Thank you for choosing Frappe-Bench Installation Script to streamline your development process. Enjoy using Frappe and happy coding!
