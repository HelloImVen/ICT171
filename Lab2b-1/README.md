## Progression for Lab2b-1

### Creating the Azure Virtual Machine.

I started by creating a new virtual machine in Microsoft Azure. I used my Azure for a Students subscription, created a resource group for this lab, named the VM `azure-webserver`, and selected the East Asia region.

![Creating Azure virtual machine](./Screenshots/Screenshot%202026-07-11%20150537.png)

### Checking the Estimated Cost.

Before creating the VM, I checked the estimated cost shown by Azure. This was important because I was using my student subscription credits, so I wanted to make sure the VM was still within the free credit amount.

![Reviewing virtual machine cost](./Screenshots/Screenshot%202026-07-11%20150603.png)

### Downloading the SSH Private Key.

Azure created an SSH key pair for the VM. I downloaded the private key because I needed it later to connect to the server from PowerShell.

![Downloading private SSH key](./Screenshots/Screenshot%202026-07-11%20150623.png)

### Starting the VM Deployment.

After checking the settings, I started the deployment. Azure then began creating the VM and the other required resources, such as the network and public IP address.

![Deployment in progress](./Screenshots/Screenshot%202026-07-11%20150824.png)

### Deployment Completed.

The deployment finished successfully. After this, Azure allowed me to go to the new virtual machine resource.

![Deployment completed](./Screenshots/Screenshot%202026-07-11%20151041.png)

### Checking the VM Overview.

I opened the VM overview page to check that the virtual machine was running. I also checked the public IP address here because I needed it later for SSH and for testing the website.

![Azure VM overview](./Screenshots/Screenshot%202026-07-11%20151105.png)

### Finding the SSH Key in PowerShell.

Next, I opened PowerShell and went to my Downloads folder. I used `dir *.pem` to check that the private key file had been downloaded.

![Finding SSH private key](./Screenshots/Screenshot%202026-07-11%20151715.png)

### Connecting to the VM Using SSH.

I used the `ssh` command with the private key file and the VM public IP address to connect to the Azure server.

![Connecting to Azure VM using SSH](./Screenshots/Screenshot%202026-07-11%20151817.png)

### Logging in to the Azure VM.

After accepting the connection prompt, I successfully logged in to the Ubuntu VM. This confirmed that the SSH key and public IP address were working.

![Logged in to Azure VM](./Screenshots/Screenshot%202026-07-11%20151833.png)

### Checking the User and Hostname.

Once I was inside the VM, I used `whoami` to check the current user and `hostname` to confirm the server name. This showed that I was logged in as `azureuser` on `azure-webserver`.

![Verifying Azure VM user and hostname](./Screenshots/Screenshot%202026-07-11%20151904.png)

### Updating Ubuntu Packages.

Before installing Apache, I updated the Ubuntu package list using `sudo apt update`. This made sure Ubuntu had the latest package information before installing new software.

![Updating Ubuntu packages on Azure VM](./Screenshots/Screenshot%202026-07-11%20154848.png)

### Installing Apache2.

I installed Apache2 using `sudo apt install apache2 -y` so the Azure VM could work as a web server. This is the software that allows the VM to show a web page in the browser.

![Installing Apache2](./Screenshots/Screenshot%202026-07-11%20154943.png)

### Checking Apache Status.

After installing Apache, I checked whether the service was running properly. The status showed that Apache was active, which meant the web server had started successfully.

![Checking Apache status](./Screenshots/Screenshot%202026-07-11%20155146.png)

### Testing the Apache Default Page.

I opened the VM public IP address in my browser. The Apache2 default page loaded, so I knew that the web server was working and could be reached from the internet.

![Testing Apache default page](./Screenshots/Screenshot%202026-07-11%20155401.png)

### Customising the Web Page.

After the default Apache page worked, I edited the web page file and replaced it with my own ICT171 cloud web server page. This made the website look more like my own lab work instead of the default Apache page.

![Viewing custom cloud web server page](./Screenshots/Screenshot%202026-07-11%20161517.png)

### Adding a GitHub Section.

I also added a GitHub section to the webpage. This showed that I could add my own content and links to the website hosted on the Azure VM.

![Viewing GitHub section on web page](./Screenshots/Screenshot%202026-07-11%20161535.png)

### My Conclusion

In this lab, I created an Ubuntu virtual machine in Microsoft Azure and used it as a simple cloud web server. I started by setting up the VM in the Azure portal, downloading the SSH private key, and then connecting to the server using PowerShell.

After I logged in to the VM, I updated Ubuntu and installed Apache2. I tested the public IP address in my browser, and the Apache default page loaded correctly. After that, I changed the default page into my own ICT171 cloud web server page and added a GitHub section.

This lab helped me understand how a cloud server is created and managed. It also gave me more practice using SSH to connect to a remote Linux server and using Apache to host a basic website.
