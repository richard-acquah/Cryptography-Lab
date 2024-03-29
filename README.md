# Cryptography-Lab

## Objectives
These cryptography labs demonstrate how to install cryptographic tools and how it is used to encrypt and decrypt files. This lab focuses on encrypting and decrypting files using __ccrypt__ and __open ssl__ in Kali Linux. This lab is a demonstration of symmetric encryption that uses a single key is used to encrypt and decrypt files.

## Skills Learned
+ File encryption and decryption.
+ Enhanced knowledge of encryption algorithms.
+ In-depth understanding of Symmetric encryption.

## Resources / Tools / Utilities
+ Kali Linux Virtual Machine
+ Ccrypt
+ Open SSL

## ENCRYPTING AND DECRYPTING FILES USING CCRYPT IN KALI LINUX
## Steps:
First update the packages in Kali Linux using the following command with elevated privileges: ***apt update***. Enter the password to proceed.

<img width="241" alt="running updatces" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/7e5b70ea-597f-42f7-9b7b-439943d61164">
<img width="400" alt="update running" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/6ffc2396-e7ab-423e-9020-97b37906d7e1">

##

Install ccrypt using the command ***apt install ccrypt*** in elevated mode. Verify the installation using the command ***ccrypt -h***: 

<img width="360" alt="ccrypt install done1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/a62b9d18-0942-4bfb-b77b-040e96d55c50">
<img width="327" alt="install verifiction1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/e064cf75-f41b-4767-876f-c6a1774890b6">

##

create a text file named mycryptotest and verify it is created. Use the ***touch*** command to create the file and verify using the ***ls*** command:

<img width="516" alt="create a file and verify2" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/bbaf4f49-8af3-4a8d-bbb5-cfa1a4930fdb">

##

Use Nano to add text to the file. The command ***nano*** mycryptotest.txt is used to open the file with a nano text editor.


<img width="158" alt="open file with nano" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/2df6f47e-47f0-43b0-a17e-8384190c7553">

<img width="646" alt="typed info in nano" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/23d87199-8fd3-41ba-b168-490521f42572">

<img width="170" alt="using cat to verify file content1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/612c905d-8d38-4fd4-870e-2a294bdc4a8d">

##

To encrypt the created file, use the command ***ccrypt*** mycryptotest and enter the encryption key:

<img width="231" alt="encrypting the file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/2d88c1a5-768a-4ad9-b595-f82109ed6863">

##

use ***ls*** to verify the encrypted file. File with cpt extension replaces the original file when the file is encrypted. The file will remain encrypted in storage and in transit.
Use nano to view the encrypted content of mycryptotest file using the command in the previous steps. The content of the file is unreadable.

<img width="351" alt="ls to view encrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/d7aef4a8-cd87-4aff-a269-99910247f3a4">

<img width="427" alt="result of opened encrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/3a9085d9-d36e-4984-ad11-e89c45236d35">


##

To decrypt the file, the command ***ccat*** is used to temporarily view the file's content without decrypting the actual file. Enter the encryption key to view the file.

<img width="380" alt="display the decrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/0e57c35e-3263-42f6-8c27-22b6385f90a4">

##

The command ***ccrypt -d*** is used to decrypt the file entirely. Enter the encryption key and the file is decrypted. Verify decryption using the ***ls*** command. 

<img width="486" alt="decrypt and ls1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/1e6cc896-272b-4f52-87fc-d38ccfe7cdcf">

##

To change the encryption key, use the command ***ccrypt -x***:

<img width="371" alt="changing key1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/51e035cc-2daf-4301-bfbc-4e04e2ba2917">

 

## ENCRYPTING AND DECRYPTING FILES USING OPEN SSL IN KALI LINUX
## Steps:
Create a text file on the desktop and name it secrete.txt. use a nano text editor to add text to the file. 

<img width="580" alt="nano edit text1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/fa94f887-c6e7-450b-ad68-e90cf7c4cb47">

##

Verify secret.txt file:

<img width="441" alt="file on desktop1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/c8c54332-a308-4a87-9f78-f945b559ddc2">

##

To encrypt secret.txt, use the command: ***openssl aes-256-cdc -a -pbkdf2 -in secret.txt -out secret.enc*** and enter and create an encryption password.

__NOTE__: enc extension means the file is encrypted.

<img width="413" alt="prompt for password1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/2c775ee5-1b18-4587-881d-20096075e9be">

##

Verify the encrypted file is created and the content with the text editor:

<img width="521" alt="enc file and content1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/72143053-d1fd-4616-8cab-e7aad983be92">

##

To decrypt the secret.enc, use the command: ***openssl aes-256-cdc -a -pbkdf2 -in secret.enc -out secret.txt*** and enter the encryption password used to encrypt the file.

__NOTE__: I deleted the original secret.txt before decrypting.


<img width="547" alt="decrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/331ddb68-227e-4cfc-a311-21e03cef2212">

## Conclusion
Encryption tools are essential in cyberspace. Network breaches are inevitable, and encrypting data in transit and storage is essential in keeping important data out of the hands of adversaries. 
