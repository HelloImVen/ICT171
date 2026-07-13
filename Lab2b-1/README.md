## Progression for Lab2b-1

### Creating the Azure Virtual Machine.

I started by creating a new virtual machine in Microsoft Azure. I used my Azure for Students subscription and created a new resource group called `rg-ict171`. I named the virtual machine `azure-webserver` and selected the East Asia region.

![Creating Azure virtual machine](./Screenshots/Screenshot%202026-07-11%20150537.png)

### Checking the Estimated Cost.

Before creating the virtual machine, I checked the estimated cost shown by Azure. The selected VM size was `Standard B2ats v2`, and the cost was covered using my Azure student subscription credits.

![Reviewing virtual machine cost](./Screenshots/Screenshot%202026-07-11%20150603.png)

### Downloading the SSH Private Key.

Azure generated an SSH key pair for the virtual machine. I downloaded the private key because it was needed to connect to the VM later using SSH.

![Downloading private SSH key](./Screenshots/Screenshot%202026-07-11%20150623.png)

### Starting the VM Deployment.

After reviewing the settings, I created the virtual machine. Azure then started deploying the VM and the required resources, such as the network and public IP address.

![Deployment in progress](./Screenshots/Screenshot%202026-07-11%20150824.png)

### Completing the VM Deployment.

The deployment completed successfully. Azure showed that the virtual machine had been created, and I was able to go to the new resource.

![Deployment completed](./Screenshots/Screenshot%202026-07-11%20151041.png)

### Checking the VM Overview.

I opened the VM overview page to check that the virtual machine was running. This page also showed important details such as the operating system, region, VM size, and public IP address.

![Azure VM overview](./Screenshots/Screenshot%202026-07-11%20151105.png)

### Finding the SSH Key in PowerShell.

Next, I opened Windows PowerShell on my computer and went to the Downloads folder. I used `dir *.pem` to confirm that the SSH private key file had been downloaded.

![Finding SSH private key](./Screenshots/Screenshot%202026-07-11%20151715.png)

### Connecting to the VM Using SSH.

I used the `ssh` command with the private key file and the VM public IP address to connect to the Azure virtual machine.

```bash
ssh -i .\azure-webserver_key.pem azureuser@104.214.189.237
