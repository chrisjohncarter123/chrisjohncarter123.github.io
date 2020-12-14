---
layout: post
title:      "Cryptography Tools"
date:       2020-12-13 00:15:21 -0500
permalink:  cryptography_tools
---


Encryption is used to hide plaintext messages into encrypted messages that cannot be understood except by the sender and receiver. It is important for securing both wired and wireless networks, and using the best tools will help implement best practices with high efficiency. Some tools used for encryption include MD5 Calculator, HashMyFiles, BitLocker, VeraCrypt, and AES Crypt. This paper will discus the following for each of these tools:
Pros and cons
Specific use cases
Their part in guarding against crypto attacks
Additional protection methods/policies

**MD5 Calculator**

	MD5 is a simple, easy to use application for calculating the MD5 hash value of a selected file. It is very quick and easy to use, but it may not have the advanced features some users need. To hash a file using MD5 Calculator, simply right click on a file and select MD5 Calculator. The program will then calculate the MD5 hash in the MD5 Digest field. This application also offers quick comparing between other hashes. To compare this MD5 digest to another, one can paste the other value into the Compare To field. Obviously, an equal sign (“=”) appears between the two values if they are equal; otherwise, the less than (“<”) or greater than (“>”) sign will tell you that the values are different.” (EC-Council 2018)
	Hashing is especially useful for passwords, or any other type of sensitive information that should not be stored as plaintext in a database.
	
**HashMyFiles**

	“HashMyFiles is small utility that allows to calculate the MD5 and SHA1 hashes of one or more files in the system. It allows to copy the MD5/SHA1 hashes list into the clipboard or save them into text/html/xml file. One can launch HashMyFiles from the context menu of Windows Explorer and display MD5/SHA1 hashes of the selected file or folder.” HasMyFiles has the advantage of being able to hash multiple files simultaneously. (EC-Council 2018)

**BitLocker**

	BitLocker is a data protection feature by Microsoft that integrates with the operating system and protects against “data theft or exposure from lost, stolen, or inappropriately decommissioned computers.” BitLocker helps mitigate unauthorized data access and also helps render data inaccessible when computers are decommissioned (Simpson et al., 2018). “BitLocker is the Windows encryption technology that protects your data from unauthorized access by encrypting your drive and requiring one or more factors of authentication before it will unlock it, whether for regular Windows use or an unauthorized access attempt” (Finding your BitLocker recovery key in Windows 10).
	BitLocker is very easy to use and requires almost no effort. It can be turned on and off easily, and no technical knowledge is required to use its features. It is developed by a large company, so it will have good support and community for good long-term stability. One slight problem of BitLocker that it requires users to have a BitLocker Recovery Key. If this key is lost, all data on the device will be completely inaccessible (zumBrunnen, 2019).

**VeraCrypt**

	VeraCrypt is developed by IDRIX (https://www.idrix.fr) and is an open source disk encryption software for Windows, OSX, and Linux. According to the VeraCrypt website, here are the main features:
“Creates a virtual encrypted disk within a file and mounts it as a real disk.
Encrypts an entire partition or storage device such as USB flash drive or hard drive.
Encrypts a partition or drive where Windows is installed (pre-boot authentication).
Encryption is automatic, real-time(on-the-fly) and transparent.
Parallelization and pipelining allow data to be read and written as fast as if the drive was not encrypted.
Encryption can be hardware-accelerated on modern processors.
Provides plausible deniability, in case an adversary forces you to reveal the password: Hidden volume (steganography) and hidden operating system." (VeraCrypt)

**AES Crypt**

	“AES Crypt is a file encryption software available on several operating systems that uses the industry standard Advanced Encryption Standard (AES) to easily and securely encrypt files.
	You do not need to be an expert to use AES Crypt, nor do you need to understand cryptography. AES Crypt is designed to be as simple to use as possible, yet still provide the strongest encryption strength available. With over a million downloads, AES Crypt has made it easy for so many people to secure information.
Using a powerful 256-bit encryption algorithm, AES Crypt can safely secure your most sensitive files. Once a file is encrypted, you do not have to worry about a person reading your sensitive information, as an encrypted file is completely useless without the password. It simply cannot be read.
	AES Crypt is the perfect tool for anyone who carries sensitive information with them while traveling, uploads sensitive files to servers on the Internet, or wishes to protect sensitive information from being stolen from the home or office. AES Crypt is also the perfect solution for those who wish to backup information and store that data at a bank, in a cloud-based storage service, and any place where sensitive files might be accessible by someone else.
	AES Crypt is free open source software. As open source, several people have contributed to and/or reviewed the software source code to ensure that it works properly to secure information. You are free to use this software in your business, at home, or in your own open source development projects.”
(AES Crypt - Advanced File Encryption)
	In conclusion, there are many great encryption tools to increase security in networks. They all have their strengths and weaknesses, and should be used 


**References:**

AES Crypt - Advanced File Encryption. (n.d.). Retrieved December 10, 2020, from https://www.aescrypt.com/

EC-Council.  (2018). Certified Ethical Hacker (CEH) Version 10 eBook w/ iLabs (Volume 4: Ethical Hacking Concepts and Methodology). [[VitalSource Bookshelf version]].

Finding your BitLocker recovery key in Windows 10. (n.d.). Retrieved December 12, 2020, from https://support.microsoft.com/en-us/windows/finding-your-bitlocker-recovery-key-in-windows-10-6b71ad27-0b89-ea08-f143-056f5ab347d6


Simpson, D., Sosnowski, R., V., V., O., Liu, J., . . . Groce, J. (2018, January 26). BitLocker. Retrieved December 10, 2020, from https://docs.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-overview

VeraCrypt. (n.d.). Retrieved December 10, 2020, from https://www.veracrypt.fr/en/Home.html

ZumBrunnen, J. (2019, February 12). BitLocker and Windows 10 Pro protect your data. Retrieved December 12, 2020, from https://community.windows.com/en-us/stories/what-is-bitlocker-windows-10


