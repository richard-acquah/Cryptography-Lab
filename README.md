# Cryptography-Lab

## Objectives
These cryptography labs demostrate how to install cryptographic tools and how it is used to encrypt and decrypt file. This lab focuses encrypting and decrypting files using ccrypt and openssl in Kali linux. The lab is a demostration of symmetric encryption and how a single key is used to encrypt and decrypt files.

## Skills Learned
+ File encryption and decryption.
+ Enhanced knowledge in encryption algorithms.
+ Indepth understanding of Symmetric encryption.

## Resources / Tools / Utilities
+ Kali Linux
+ Ccrypt
+ Openssl

## ENCRYPTING AND DECRYPTING FILES USING CCRYPT IN KALI LINUX
## Steps:
First update the packages in kali linux using the following command with elivated privillages: apt update. Enter password to proceed.
<img width="241" alt="running updatces" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/7e5b70ea-597f-42f7-9b7b-439943d61164">
<img width="400" alt="update running" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/6ffc2396-e7ab-423e-9020-97b37906d7e1">

Install ccrypt using the command apt install ccrypt in elivated mode. Verify the installation using the command ccrypt -h: 

<img width="360" alt="ccrytp install done1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/a62b9d18-0942-4bfb-b77b-040e96d55c50">
<img width="327" alt="install verifiction1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/e064cf75-f41b-4767-876f-c6a1774890b6">

create text file named mycryptotest and verify it is created. Use the touch command to create the file and verify using the ls command:

<img width="516" alt="creat a file and verify2" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/bbaf4f49-8af3-4a8d-bbb5-cfa1a4930fdb">


Use nano to add text to the file. The command nano mycryptotest.txt to open the file with nano text editor:
