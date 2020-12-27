---
layout: post
title:      "Some Encryption Tools"
date:       2020-12-27 21:48:10 +0000
permalink:  some_encryption_tools
---


**BitLocker**
BitLocker is a data protection feature by Microsoft that integrates with the operating system and protects against “data theft or exposure from lost, stolen, or inappropriately decommissioned computers.” BitLocker helps mitigate unauthorized data access and also helps render data inaccessible when computers are decommissioned (Simpson et al., 2018). “BitLocker is the Windows encryption technology that protects your data from unauthorized access by encrypting your drive and requiring one or more factors of authentication before it will unlock it, whether for regular Windows use or an unauthorized access attempt” (Finding your BitLocker recovery key in Windows 10). 

BitLocker is very easy to use and requires almost no effort. It can be turned on and off easily, and no technical knowledge is required to use its features. It is developed by a large company, so it will have good support and community for good long-term stability. One slight problem of BitLocker that it requires users to have a BitLocker Recovery Key. If this key is lost, all data on the device will be completely inaccessible (zumBrunnen, 2019). The only supported operating system is Windows, so it is not an option for Mac or Linux users.

**VeraCrypt**
VeraCrypt is developed by IDRIX (https://www.idrix.fr) and is an open-source disk encryption software for Windows, OSX, and Linux. According to the VeraCrypt website, here are the main features:
“Creates a virtual encrypted disk within a file and mounts it as a real disk.
Encrypts an entire partition or storage device such as USB flash drive or hard drive.
Encrypts a partition or drive where Windows is installed (pre-boot authentication).
Encryption is automatic, real-time(on-the-fly) and transparent.
Parallelization and pipelining allow data to be read and written as fast as if the drive was not encrypted.
Encryption can be hardware-accelerated on modern processors.
Provides plausible deniability, in case an adversary forces you to reveal the password: Hidden volume (steganography) and hidden operating system."
(VeraCrypt)

VeraCrypt may be a better alternative to BitLocker for non-windows machines. It may require a little more human work than BitLocker.
	
**AES Crypt**
AES Crypt is a great tool to encrypt files with sensitive information with a password. “AES Crypt is a file encryption software available on several operating systems that uses the industry standard Advanced Encryption Standard (AES) to easily and securely encrypt files.

You do not need to be an expert to use AES Crypt, nor do you need to understand cryptography. AES Crypt is designed to be as simple to use as possible, yet still provide the strongest encryption strength available. With over a million downloads, AES Crypt has made it easy for so many people to secure information.
Using a powerful 256-bit encryption algorithm, AES Crypt can safely secure your most sensitive files. Once a file is encrypted, you do not have to worry about a person reading your sensitive information, as an encrypted file is completely useless without the password. It simply cannot be read.

AES Crypt is the perfect tool for anyone who carries sensitive information with them while traveling, uploads sensitive files to servers on the Internet, or wishes to protect sensitive information from being stolen from the home or office. AES Crypt is also the perfect solution for those who wish to backup information and store that data at a bank, in a cloud-based storage service, and any place where sensitive files might be accessible by someone else.

AES Crypt is free open source software. As open source, several people have contributed to and/or reviewed the software source code to ensure that it works properly to secure information. You are free to use this software in your business, at home, or in your own open source development projects.” (AES Crypt - Advanced File Encryption)

One drawback of AES Crypt is that it does not support multi-factor authentication, something many companies may require for very important information.

In conclusion, there are many great encryption tools to increase security in networks. They all have their strengths and weaknesses and should be used efficiently to maximize productivity.

**References:**

AES Crypt - Advanced File Encryption. (n.d.). Retrieved December 10, 2020, from https://www.aescrypt.com/ 
EC-Council. (2018). 

Finding your BitLocker recovery key in Windows 10. (n.d.). Retrieved December 12, 2020, from https://support.microsoft.com/en-us/windows/finding-your-bitlocker-recovery-key-in-windows-10-6b71ad27-0b89-ea08-f143-056f5ab347d6

Simpson, D., Sosnowski, R., V., V., O., Liu, J., . . . Groce, J. (2018, January 26). BitLocker. Retrieved December 10, 2020, from https://docs.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-overview

VeraCrypt. (n.d.). Retrieved December 10, 2020, from https://www.veracrypt.fr/en/Home.html

ZumBrunnen, J. (2019, February 12). BitLocker and Windows 10 Pro protect your data. Retrieved December 12, 2020, from https://community.windows.com/en-us/stories/what-is-bitlocker-windows-10







