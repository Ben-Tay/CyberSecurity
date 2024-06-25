## Device Hardening
> Process of securing a device to minimize vulnerabilities.

More layers of security = safer device

Harden by:
1. Disabling unneeded features
2. Updating firmware, OS and software
3. Using firewalls, VPN and anti-malware

#### Apps and OSes
* Turn on auto-updates for PCs, phones, tablets and routers to protect apps and OSes

Outdated systems are huge targets for hackers:
* Unpatched (missing updates)
* Unsupported (no VPN/antivirus)
* Old, unsupported OS
* Employee personal computers (no security apps)

Do the following:
* Install apps only from trusted resellers, app stores
* Check digital signatures of app beforehand
* Updated regularly

## Patching updates
> Patches are updates to apps and OSes that fix security weaknesses (Known threats - alr happened)

Companies regularly release patches alongside
system improvement updates to make sure that their customers are safe from new threats.

To fight against unknown theeats:
* Use MFA
* VPN
* Strong passwords

## Firmware updates
Firmware is `software` that tells hardware how to behave.

Security firmware protects devices and data from malware and tampering.

#### BIOS/Firmware passwords
* Aka Basic Input Output System
* Firmware that is used to boot up Windows & Linux PCs
* Runs hardware checks and starts the OS
* OS won't start without the password or if the checks find a problem

#### UEFI (Unified Extensible Firmware Interface)
* Newer and more advanced boot firmware than BIOS
* Secure boot is a feature of UEFI
* It confirms an OS manfacturer's digital signature preventing malware from `taking control` during boot-up.

#### Trusted Platform Model (TPM)
* Chip that stores and manages encryption keys
* Won't start a device or unencrypt data if tampering is detected

#### Drive Encryption
* Scrambles a drive data so it is unreadable
> Ensure all devices have updated firmware

## Encryption
> One of the most powerful tools you can use to harden a device.

* Uses algorithm to encrypt plain text into unreadable ciphertext, which can only be decoded by encryption key

* Used at network layer for data travelling across networks, and be can done locally to `hard drives, phones and thumb drives` so that lost device data remains unreadable.

## Disable features and ports
A Hacker can use features and ports to steal data and cause damage.

#### Features
`Autorun` allows inserted drives and disks to run or play automatically - `could run malware`

`Bluetooth` is vulnerable to data interception

`NFC` has zero security except for its limited range

#### Ports
`Port 443`  manages secure web traffic (HTTPS)

`Port 22` used for secure server connections (SSH)

`Port 80` used for standard web traffic (HTTP)

> To harden against attack, disable unused features and ports, and use other hardening tools to protect the ones in use.

## Zero-Day attacks
> A zero-day attack is an attack that has never happened before.

> There are no patches or updates in a zero-day attack because they haven’t been created yet.

To protect against zero-day attacks:'
* Use tools like VPN and IDS/IPS
* Visit only trusted networks and sites

## Firewalls and VPNS
Firewalls harden devices by keeping unwanted visitors out of your system and off your network.
* Consists of software and hardware firewalls
* Blocks harmful traffic based on preset rules

#### Software Firewalls
*  Host-based firewalls are programs that are installed on a computer. 
* Most modern operating systems have built-in firewall software. 
* Microsoft, for example, provides Windows Defender Firewall. These built-in firewalls help to monitor port traffic and traffic between applications.

#### Hardware Firewalls
* network-based firewalls are deployed between a network and an internet gateway 
* In-home or small business settings, a router often has built-in firewall protection to stop unwanted traffic from the outside.
* Larger organizations use separate firewall devices to protect their network

#### How firwalls work
`Packet Filtering`
*  firewall that uses packet filtering reviews each packet that tries to access a network or device
* Any packets that match known threats or that have been explicitly denied are removed and all other packets are sent through to their destination. 

` Stateful Inspection/Dynamic Filtering`
* monitors the state of active network connections
* relies on patterns to analyze and monitor traffic for potential threats.

` Proxy Firewall`
* Acts as a go-between for the requesting system and the internet. 
* Information is first sent to the proxy service before it is forwarded to its destination

`Filters`
* Firewalls can be configured to meet the specific need of an individual or organization. 
* Traffic can be approved or denied based on IP addresses, ports, domain names, and even specific words and phrases

VPNs encrypt traffic so it cant be read.
* Use VPNs in conjunction with public wifi (if necessary)

`Domain network`:
*  Domain networks are workplace networks. A computer must be a part of the domain in order to communicate with other computers on that network.

`Private network`: 
* Private networks are discoverable networks, meaning that only devices on that network can see or discover other devices on that same network. Home networks are a good example of a private network.

`Public network`: 
* Public networks are non-discoverable networks. A non-discoverable network is a network where your device cannot be discovered by other devices on your network. A coffee shop or a library would be a good example of a public network. You do not want other individuals to be able to discover your device.