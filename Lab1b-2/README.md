### Verifying the New Users

The new user accounts for Alice, Bob, and Mallory were checked to make sure they existed on the system.

![Verifying users were created](./Screenshots/Screenshot%202026-07-10%20150949.png)

### Checking the `sharedgroup` Members

The `sharedgroup` membership was checked to confirm that Alice and Bob were included. This group was used to control access to the shared folder.

![Checking sharedgroup members](./Screenshots/Screenshot%202026-07-10%20151156.png)

### Setting Permissions for `/home/shared`

The ownership of `/home/shared` was changed so Alice was the owner and `sharedgroup` was the group. The permissions were then updated so access could be tested properly.

![Setting ownership and permissions](./Screenshots/Screenshot%202026-07-10%20151713.png)

### Testing Alice’s Access

Alice was able to list the files in `/home/shared` and write to a shared file. This confirmed that Alice had the correct owner permissions.

![Alice writing to shared file](./Screenshots/Screenshot%202026-07-10%20152042.png)

### Testing Bob’s Access

Bob was able to access and read the shared file because he was part of `sharedgroup`. However, when Bob tried to write to the file, the system returned `Permission denied`.

![Bob permission denied](./Screenshots/Screenshot%202026-07-10%20152820.png)

### Testing Mallory’s Access

Mallory was not part of `sharedgroup`, so she was denied access when trying to list or read files in `/home/shared`.

![Mallory permission denied](./Screenshots/Screenshot%202026-07-10%20153211.png)

### Testing Sudo Access with Mallory

Mallory was added to the `sudo` group to test administrator permissions. After this, Mallory was able to use `sudo` to access restricted directories.

![Mallory sudo access](./Screenshots/Screenshot%202026-07-10%20153451.png)
