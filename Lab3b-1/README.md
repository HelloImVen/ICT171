## Progression for Lab3b-1

### Updating Ubuntu Packages.

I started by running `sudo apt update` on the Azure Ubuntu VM. I did this first so the package list was up to date before installing anything needed for the backup lab.

![Updating Ubuntu packages](./Screenshots/Screenshot%202026-07-11%20171605.png)

### Installing Zip and Cron.

I installed `zip` and `cron` because this lab needed zip files for backups and cron for scheduled tasks. The terminal showed that cron was already installed and zip was added successfully.

![Installing zip and cron](./Screenshots/Screenshot%202026-07-11%20171647.png)

### Enabling Cron.

I enabled the cron service so it could start automatically when the server starts. This was needed because the backup script would later be scheduled using cron.

![Enabling cron](./Screenshots/Screenshot%202026-07-11%20171742.png)

### Starting and Checking Cron.

I started cron and checked its status. The output showed that `cron.service` was active and running, which meant the scheduled task service was working.

![Starting and checking cron](./Screenshots/Screenshot%202026-07-11%20171844.png)

### Practising Basic Bash Commands.

I practised a few Bash commands using variables, simple maths, and a loop. I made a small mistake with the `do` part of the loop, but the final output still showed the correct sum from 1 to 5.

![Practising basic Bash commands](./Screenshots/Screenshot%202026-07-11%20172425.png)

### Creating Test Files for Backup.

I created a `Documents` folder with test files and also made a `testfolder` inside it with more files. I used `ls -R` to check that the folder structure and files were created properly.

![Creating test files for backup](./Screenshots/Screenshot%202026-07-11%20173147.png)

### Writing the Backup Script.

I created a backup script called `testscript` using `nano`. The script was written to copy files from the `Documents` folder, place them into a backup folder, and then compress the backup into a zip file with the date and time in the filename.

![Writing backup script](./Screenshots/Screenshot%202026-07-11%20173617.png)

### Running the Backup Script.

I gave the script permission to run and executed it. The script copied the files into the backup folder and created a zip backup file.

![Running backup script](./Screenshots/Screenshot%202026-07-11%20173757.png)

### Checking the Created Backup File.

I checked the home directory for zip files and confirmed that the backup file was created successfully.

![Checking created backup file](./Screenshots/Screenshot%202026-07-11%20174042.png)

### Moving the Script to `/usr/bin`.

I moved the backup script into `/usr/bin` and changed its permissions so it could be run like a normal command. I then ran `testscript` again and confirmed that another backup zip file was created.

![Moving script to usr bin](./Screenshots/Screenshot%202026-07-11%20174408.png)

### Adding the Script to Cron.

I edited `/etc/crontab` and added a cron job for the backup script. This was done so the script could run automatically on a schedule instead of needing to run it manually each time.

![Adding script to cron](./Screenshots/Screenshot%202026-07-11%20174544.png)

### Restarting Cron and Checking Status.

After editing the crontab file, I restarted cron and checked its status again. The output showed that cron was active and running, so the scheduled backup setup was ready.

![Restarting cron and checking status](./Screenshots/Screenshot%202026-07-11%20175050.png)

### My Conclusion

In this lab, I created a simple backup system on my Azure Ubuntu server. I started by installing the tools needed for the lab, including `zip` and `cron`. After that, I made sure cron was enabled and running properly.

I then created test files inside the `Documents` folder so there was something to back up. After that, I wrote a backup script called `testscript`. The script copied the files into a backup folder and compressed them into a zip file with the date and time in the filename. I tested the script manually first to make sure it worked.

After the script worked, I moved it into `/usr/bin` and added it to `/etc/crontab` so it could run automatically. This lab helped me understand how Linux backup scripts work and how cron can be used to schedule tasks on a server.
