# Cryptography-Lab

## Objectives
These cryptography labs demostrate how to install cryptographic tools and how it is used to encrypt and decrypt file. This lab focuses encrypting and decrypting files using __ccrypt__ and __open ssl__ in Kali linux. The lab is a demostration of symmetric encryption and how a single key is used to encrypt and decrypt files.

## Skills Learned
+ File encryption and decryption.
+ Enhanced knowledge in encryption algorithms.
+ Indepth understanding of Symmetric encryption.

## Resources / Tools / Utilities
+ Kali Linux
+ Ccrypt
+ Open ssl

## ENCRYPTING AND DECRYPTING FILES USING CCRYPT IN KALI LINUX
## Steps:
First update the packages in kali linux using the following command with elivated privillages: ***apt update***. Enter password to proceed.
<img width="241" alt="running updatces" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/7e5b70ea-597f-42f7-9b7b-439943d61164">
<img width="400" alt="update running" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/6ffc2396-e7ab-423e-9020-97b37906d7e1">

Install ccrypt using the command ***apt install ccrypt*** in elivated mode. Verify the installation using the command ***ccrypt -h***: 

<img width="360" alt="ccrytp install done1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/a62b9d18-0942-4bfb-b77b-040e96d55c50">
<img width="327" alt="install verifiction1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/e064cf75-f41b-4767-876f-c6a1774890b6">

create text file named mycryptotest and verify it is created. Use the ***touch*** command to create the file and verify using the ***ls*** command:

<img width="516" alt="creat a file and verify2" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/bbaf4f49-8af3-4a8d-bbb5-cfa1a4930fdb">


Use nano to add text to the file. The command ***nano*** mycryptotest.txt to open the file with nano text editor.


<img width="158" alt="open file with nano" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/2df6f47e-47f0-43b0-a17e-8384190c7553">

<img width="646" alt="typed info in nano" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/23d87199-8fd3-41ba-b168-490521f42572">

<img width="170" alt="using cat to verify file content1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/612c905d-8d38-4fd4-870e-2a294bdc4a8d">

To encrypt the created file, use the command ***ccrypt*** mycryptotest and enter encryption key:

<img width="231" alt="encrypting the file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/2d88c1a5-768a-4ad9-b595-f82109ed6863">

use ***ls*** to verify the encrypted file. File with cpt extension replaces the original file when the file is encrypted. The file will remain encrypted in storage and in transit.
Use nano to view the encrypted content of mycryptotest file using the command in the previouse steps. The content of the file unreadable.

<img width="351" alt="ls to view encrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/d7aef4a8-cd87-4aff-a269-99910247f3a4">

<img width="427" alt="result of opened encrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/3a9085d9-d36e-4984-ad11-e89c45236d35">

To decrypt the file, the command ***ccat*** is used to temporary view the content of the file without decrypting the actual file. Enter the encryption key to view the file.

<img width="380" alt="display the decrypted file1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/0e57c35e-3263-42f6-8c27-22b6385f90a4">

To  decrypt the file entirely, the command ***ccrypt -d*** is used. Enter the encryption key and the file is decrypted. Verify decryption using the ***ls*** command. 

<img width="486" alt="decrypt and ls1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/1e6cc896-272b-4f52-87fc-d38ccfe7cdcf">

To change encryption key, use the command ***ccrypt -x***:

<img width="371" alt="changing key1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/51e035cc-2daf-4301-bfbc-4e04e2ba2917">

## Conclusion
Encryption tools are essential in the cyberspace. Network breaches are inevitable and encrypting data in tansit and in storage is essential in keeping important data out of the hands os adversaries.  



## ENCRYPTING AND DECRYPTING FILES USING OPEN SSL IN KALI LINUX
## Steps:
Create text file on desktop and name it secrete.txt. use nano text editor to add text to the file. 

<img width="580" alt="nano edit text1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/fa94f887-c6e7-450b-ad68-e90cf7c4cb47">

Verify secret.txt file:

<img width="441" alt="file on desktop1" src="https://github.com/richard-acquah/Cryptography-Lab/assets/136107996/c8c54332-a308-4a87-9f78-f945b559ddc2">





