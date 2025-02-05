# Digital Security Tips
ranked in no particular order: 

1. Always enable 2FA to secure your accounts whenever possible. There are many 2FA options available but the most secure one is going to be a hardware authenticator such as a Yubikey which you can buy online for around $50. If you can't spend money and need a free option, you can opt for a software TOTP authenticator app instead (I recommend 2FAS authenticator app for Android/iOS). Some websites don't support both hardware and software TOTP authenticators, in which case your only option is to use either Email 2FA or SMS 2FA as a last resort. Email 2FA and SMS 2FA should only be used when all other options are unavailable as they aren't very secure. 

2. Make sure you're using strong passwords and never reuse the same password for multiple accounts. To ensure that your passwords are strong and unique, use a password manager (I recommend an offline one such as KeePassXC for Windows/macOS/Linux, KeePassDX for Android, and KeePassium for iOS) to help generate unique and randomized passwords and store them for you. For the password manager's master password, make sure to use a randomly-generated Diceware passphrase consisting of at least 6 words (10 words if you want maximum security, although this would be harder to memorize). Your passwords should only exist within your password manager, do not store/save them anywhere else and do not share them with anyone else. Immediately change your password in the event of a data breach or if you suspect one of your accounts was compromised. 

3. Be wary of phishing/malicious links/URLs and do not open files sent by strangers. If you really have to open the file, make sure to open it in an isolated VM/sandbox (such as VirtualBox). Also make sure to only install software from trusted and reputable sources and review their permissions before installing. 

4. Never enter your credentials or any other sensitive information on websites that are not secured by HTTPS. HTTP websites are unencrypted so anyone can easily eavesdrop on your connection. You can verify if a connection is HTTP or HTTPS by looking at the URL. Modern browsers would also display a warning for unsecured connections. Some browsers offer an HTTPS-only mode option in the settings that allows only secured connections, its a good idea to enable this option. It's important to note though, that HTTPS only protects you from a third party listening in, but not from the website itself, so you'll still have to verify if the website is trustworthy even if the website has HTTPS enabled. 

5. Make sure to log out of your accounts as soon as you are done using them. This minimizes the risk of session hijacking and prevents unauthorized access from people you're sharing the device with. 

6. When communicating sensitive information to someone else digitally, use a platform that supports end-to-end encryption (I recommend Signal for instant messaging and Proton Mail for Email) and make sure to enable self-destructing/disappearing messages whenever possible to ensure that message history is erased from both sender and recipient accounts. 

7. If you're accessing the internet through a public Wi-Fi (for example a cafe Wi-Fi), it's recommended to do it while using a trusted and reputable VPN service (I recommend Proton VPN). Otherwise, whenever possible, it's best to use your own password-protected mobile data tethering when out in public. 

8. Keep all your critical software and firmware up to date to get the latest security patches. 

9. Do not upload sensitive files/data on the cloud or any other web service. Its best to keep all sensitive data offline to eliminate the risk of a hacker compromising the server and stealing your secrets. If you're forced to resort to cloud backups, make sure they're end-to-end encrypted (I recommend using encryption software like Cryptomator or VeraCrypt to ensure this). 

10. Enable full-disk encryption to protect your data locally using a disk encryption software such as BitLocker for Windows, FileVault for macOS, and LUKS for Linux. On top of this, make sure to store all your sensitive files in an encrypted and password-protected folder/container on your device (e.g., with VeraCrypt or Cryptomator).
