## Progression for Lab2b-2

### Opening the LabFiles Folder.

I started by going into the `LabFiles` folder on the Azure Ubuntu VM. The folder already existed as i was redoing the lab for my screenshots, so I just changed into it and continued the lab from there.

![Opening LabFiles folder](./Screenshots/Screenshot%202026-07-11%20162009.png)

### Creating and Testing a Notes File.

I created a simple `notes.txt` file for the Bash scripting lab and checked the contents using `cat`. I also practised copying and renaming files. At first, I made a small mistake by typing the file name like a command, but after that I checked the folder contents with `ls -l`.

![Creating and testing notes file](./Screenshots/Screenshot%202026-07-11%20162318.png)

### Fixing the File Rename and Remove Commands.

After noticing the earlier mistake, I used the correct `mv` command to rename the backup file and then removed it. The final `ls -l` showed that only `notes.txt` was left in the folder.

![Fixing file commands](./Screenshots/Screenshot%202026-07-11%20162703.png)

### Creating the Hello World Script.

I created a Bash script called `hello_world.sh` using `nano`. The script prints “Hello World”, a short message for ICT171, the current user, and the current directory.

![Creating hello world script](./Screenshots/Screenshot%202026-07-11%20162756.png)

### Checking the Script File.

I listed the files in the folder using `ls -l` to check that `hello_world.sh` and `notes.txt` were both saved in the `LabFiles` folder.

![Checking script file](./Screenshots/Screenshot%202026-07-11%20162831.png)

### Viewing the Hello World Script.

I used `cat hello_world.sh` to display the contents of the script in the terminal. This helped confirm that the script was saved correctly.

![Viewing hello world script](./Screenshots/Screenshot%202026-07-11%20162855.png)

### Creating the Number Check Script.

Next, I created another Bash script called `number_check.sh`. This script uses a loop to check numbers from 1 to 5 and prints a message when number 3 is found.

![Creating number check script](./Screenshots/Screenshot%202026-07-11%20163016.png)

### Running the Number Check Script.

I made the script executable using `chmod +x number_check.sh` and then ran it. The output showed each number being checked, and it correctly detected number 3.

![Running number check script](./Screenshots/Screenshot%202026-07-11%20163151.png)

### Creating the Resource Monitor Script.

I created a third Bash script called `resource_monitor.sh`. This script was made to show basic system information such as the date and time, CPU/process information, memory usage, and disk usage.

![Creating resource monitor script](./Screenshots/Screenshot%202026-07-11%20163317.png)

### Running the Resource Monitor Script.

I made `resource_monitor.sh` executable and ran it. The script started by showing the date and time, followed by CPU and process information from the system.

![Running resource monitor script](./Screenshots/Screenshot%202026-07-11%20163551.png)

### Checking Memory and Disk Usage Output.

The rest of the script output showed memory usage and disk usage. This confirmed that the script was able to collect and display useful system resource information.

![Checking memory and disk usage output](./Screenshots/Screenshot%202026-07-11%20163613.png)

### My Conclusion

In this lab, I practised creating and running Bash scripts on my Azure Ubuntu virtual machine. I started by working with simple files in the `LabFiles` folder, including creating, copying, renaming, and removing text files. I also made a small mistake while renaming a file, but I corrected it by using the proper command afterwards.

After that, I created a few Bash scripts. The first script printed a simple message and showed the current user and directory. The second script used a loop to check numbers and find number 3. The last script worked like a basic resource monitor by showing the date, CPU/process information, memory usage, and disk usage.

This lab helped me understand how Bash scripts can automate tasks in Linux. It also gave me more practice using commands like `nano`, `cat`, `chmod`, and running scripts from the terminal.
