## Progression for Lab1b-3

### Creating the Lab Folder and Checking the Windows User Directory.

![Creating lab folder and checking Windows directory](./Screenshots/Screenshot%202026-07-10%20160141.png)

I created the lab folder for `1b-3` and checked the Windows user directory through `/mnt/c/Users`. This helped me locate where the downloaded Gutenberg archive is stored.

### Copying the Gutenberg Archive into the Lab Folder.

![Copying Gutenberg archive](./Screenshots/Screenshot%202026-07-11%20062521.png)

The Gutenberg archive was than copied from the Windows Downloads folder into my Linux lab folder. I then used `ls -lh` to confirm that the archive was in the correct location.

### Extracting the Gutenberg Archive.

![Extracting Gutenberg archive](./Screenshots/Screenshot%202026-07-11%20062710.png)

The archive was extracted using Linux archive commands. After extraction, the text files were available for searching and analysis.

### Checking the Extracted Files.

![Checking extracted files](./Screenshots/Screenshot%202026-07-11%20062731.png)

I listed the files in the lab folder to confirm that the Gutenberg files had been extracted correctly.

### Listing Files Inside the Gutenberg Folder.

![Listing files inside Gutenberg folder](./Screenshots/Screenshot%202026-07-11%20063052.png)

I used command `ls -l Gutenberg | head` to view the files inside the Gutenberg folder. This showed the file names, permissions, owners, file sizes, and dates.

### Checking the Lab Folder Contents.

![Checking lab folder contents](./Screenshots/Screenshot%202026-07-11%20063619.png)

I checked the contents of the `1b-3` folder again to confirm that the archive, extracted folder, and text files were present.

### Finding Text Files Using `find`.

![Finding text files using find](./Screenshots/Screenshot%202026-07-11%20064549.png)

I searched for `.txt` files inside the Gutenberg folder using the `find` command. confirming that the available text files.

### Searching for `verdigris` Using `grep`.

![Searching for verdigris](./Screenshots/Screenshot%202026-07-11%20064744.png)

I used the `grep` command to search for the word `verdigris` inside the Gutenberg files. The result showed `0`, meaning the word was not found in the available files.

### Searching by Phrase, File Size, and File Date.

![Searching by phrase size and date](./Screenshots/Screenshot%202026-07-11%20064944.png)

I went on to test more search commands using `grep` and `find`, I searched for a phrase, checked for files with a specific size, and listed files by date using `find` with sorting.

### Checking File Sizes.

![Checking file sizes](./Screenshots/Screenshot%202026-07-11%20065124.png)

I used `du -a Gutenberg | sort -nr | head` to check the size of the Gutenberg folder and the text files. This helped identify the largest files.

### Running Word Frequency Analysis.

![Running word frequency analysis](./Screenshots/Screenshot%202026-07-11%20065152.png)

I used `sed`, `sort`, `uniq -c`, and `head` to perform a simple word frequency analysis on `frankenstein.txt`. This showed how Linux commands can be combined to process and analyse text.

### My Conclusion

In this lab, I practised using Linux command-line tools to search and analyse text files. I copied and extracted the Gutenberg archive, listed files, searched for text using `grep`, found files using `find`, checked file sizes using `du`, and performed word frequency analysis using commands such as `sed`, `sort`, and `uniq`.

The Gutenberg archive available to me contained only three text files: `frankenstein.txt`, `moby.txt`, and `twocities.txt`. Because of this, i could not answer exactly what some lab question asked. However, I was still able to complete the main search and analysis tasks using the files that were available to me. This lab helped me understand how Linux commands can be combined to search, filter, and analyse text files efficiently.
