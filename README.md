# Ultimate Wii Modding Guide

## Updates

- I'll try to customize the text and add other useful stuff.
- if i had a wii i could also add pictures (idk if i want to buy one)

# What you need

1. a Wii (not the Wii Mini)
2. an SD card (at least 4GB)
3. a PC or laptop to edit data on the SD card

# SD card preparation

## Windows:

To format the SD card to `Fat32`, follow the steps below:

1. right click on the SD card and select `Format`.
2. select `Fat32` as the file system and click on `Format`. 
   
   **Note:** If "Fat32" is not displayed as an option, open the command prompt (cmd) as administrator and execute the following commands:

   ```sh
   diskpart
   list disk
   sel disk 2 // Select the number of the SD card, e.g. disk 2
   format fs=fat32 quick

If you have an SD card that is larger than 32 GB and your Wii does not recognize it, download the program "Fat32 Format" (from any source). Select your SD card and set the size to 32768 to limit it to 32 GB.

## Linux:

To format the SD card in Linux, follow these steps:

1. open the terminal and run `lsblk` to get the disk information.
2. select the SD card by typing `sudo fdisk /dev/disk1` (replace `disk1` with the actual name of the SD card)
3. run this command to format the partition to FAT32:

   ```bash
   sudo mkfs.vfat -F 32 /dev/disk1

## MacOS:

To format the SD card to FAT32 in MacOS, follow these steps:

1. open the terminal and type `diskutil list` to get the info for the disk.
2. unmount the SD card first with `diskutil unmountDisk /dev/disk1` (replace `disk1` with the actual name of the SD card).
3. then execute the command to format the SD card to FAT32: `diskutil eraseDisk FAT32 nameofthesdcard MBRFormat /dev/disk1`.

# Wii preparation

1. go to "Wii options" at the bottom right of the home menu on your Wii.
2. select "Wii settings".
3. Scroll right to "Internet".
4. then go to "Console Information".
5. memorize the "MAC address" of the Internet connection you are currently using and do not share it with anyone you do not trust.
6. pack the SD card into your PC.

# SD card setup

1. go to the Letterbomb website [letterbomb](https://please.hackmii.com/)
2. enter your "MAC address" there.
3. make sure your console version is correct (U: NTSC-U, E: PAL/European, J: Japanese, K: Korean).
4. then select the correct version and make sure that `Bundle the HackMii Installer for me!
5. then click on `Cut the red wire` or `Cut the blue wire` (both options do the same).
6. now drag the `private` folder and the `boot.elf` file to the root directory of the SD card.
7. put the SD card back into your Wii.

# Loading the payload

1. go to the "Wii Message Board" at the bottom right of your Wii.
2. scroll a little to the left and right until you find a letter with a bomb.
3. select the letter with the bomb and wait.
4. in the `HackMii Installer` select "Continue" and then "Install the Homebrew Channel" and select "Yes, continue".
5. then select "Continue" and then "Exit" to enter the Homebrew Launcher.



### THIS IS ONLY AN ENGLISH TRANSLATION AND IS PROBABLY NOT PERFECT AS I WROTE THE ORIGINAL IN GERMAN.

Translated with DeepL.com (free version)
