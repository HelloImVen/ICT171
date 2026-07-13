### Verifying the New Users

Checking that the user accounts for Alice, Bob, and Mallory were added to the system.

![Verifying users were created](./Screenshots/Screenshot%202026-07-10%20150949.png)

### Checking the Members in `sharedgroup` 

The Checking if user Alice and Bob were added to `sharedgroup`. This group was used to control access to the shared folder.

![Checking sharedgroup members](./Screenshots/Screenshot%202026-07-10%20151156.png)

### Setting Permissions for `/home/shared`

Changing ownership of `/home/shared` to Alice. Permissions were then updated so access could be tested properly.

![Setting ownership and permissions](./Screenshots/Screenshot%202026-07-10%20151713.png)

### Testing Alice’s Access

Alice was able to list the files in `/home/shared` and write to a shared file. This confirmed that Alice had the correct owner permissions.

![Alice writing to shared file](./Screenshots/Screenshot%202026-07-10%20152042.png)

### Testing Bob’s Access

Bob was able to access and read the shared file because he was part of `sharedgroup`. However, when Bob tried to write to the file, the system returned `Permission denied` as he did not have access to write the file.

![Bob permission denied](./Screenshots/Screenshot%202026-07-10%20152820.png)

### Testing Mallory’s Access

Mallory was not part of `sharedgroup`, so she was denied access when trying to list or read files in `/home/shared`.

![Mallory permission denied](./Screenshots/Screenshot%202026-07-10%20153211.png)

### Testing Sudo Access with Mallory

Mallory was given administrator/root permissions. After, Mallory was able to use `sudo` command to access restricted directories.

![Mallory sudo access](./Screenshots/Screenshot%202026-07-10%20153451.png)

### My Conclusion

In this lab, I learned and practised some basic Linux commands such as whoami, pwd, and ls. 
I also used commands such as uname, lsb_release, and hostnamectl for checking system information, Explored networking tools such as ip a, ping, nslookup, and whois. 
Lastly, I used the gcc command to compile and run a simple C program. 
Overall, i feel this lab improved my understanding of how the Linux command line can be used to help file management, system monitoring, networking, and software development. 
Further more it also helped me become more confident in using Ubuntu through the command line in WSL.
