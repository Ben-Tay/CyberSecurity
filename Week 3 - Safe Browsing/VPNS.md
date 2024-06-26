## Virtual Private Networks (VPNs)
> A virtual private network (or VPN) is an encrypted tunnel set up between two or more sites.
* All traffic in the tunnel is unreadable and useless to anyone who might try to intercept the traffic.
* VPN traffic is `encrypted at the originating site` and decrypted at the receiving site.
* VPNs make it much more difficult for hackers to make eavesdropping attacks, man in the middle attacks, and replay attacks.
* VPNs can be hardware based or software based.

## Site-2-Site VPN
> Site-to-site VPN is when two sites connect across an existing internet connection with a VPN device.
* Each site’s internal network traffic is unencrypted.
* Traffic that needs to traverse the internet is encrypted by the origination site’s VPN
and then decrypted by the receiving site’s VPN device

## Host-2-site VPN
> Host-to-site VPN is when a remote user needs to connect securely to a site
* Host device uses VPN software while the site uses a VPN device or software to `protect its internal network`
* Traffic that needs to traverse the internet is encrypted by the sender’s VPN, and then decrypted by the receiver’s VPN, which then receives the traffic if the host is the receiver or routes it to its intended recipient if the site is the receiver.

## Host-2-Host VPN
> When two remote users need to connect securely to each other. This is a user-to-user or device-to-device interaction that `doesn’t require a complex encryption` solution.
* Both host devices uses VPN software
* Traffic that needs to traverse the internet is encrypted by the sender’s VPN, and then decrypted by the receiver’s VPN.

## VPN Hardware Devices
* Devices specifically designed to create virtual private networks
* Or they are existing network devices with `built-in VPN` functionality.
* Eg: Routers, Firewalls
* `VPN Concentrators`-can create and manage many VPN connections at once
* Useful for `Site-2-Site vpn`.

## VPN Software 
* Included in:
    1. Virtual LANS
    2. Operating systems and browsers (MacOs, Windows Os, Ms Edge)

## Internet Protcol Security (IPsec)
> Suite of network standards and protocols
that use cryptography to protect data traveling over the Internet.

IPsec suite core protocols:
1. `IPSec Authentication Header (AH) protocol`
    * Authenticates sender and IP addresses
2. `Encapsulating Security Payload (ESP) protocol`
    * Encrypts data and authenticates data and senders

IPsec Has 2 modes:

`Tunnel Mode`:
* Entire data packet is wrapped in a new packet, encrypted and `given` a new header
* Common in `Site-2-Site` VPN 

`Transport Mode`:
* IP header of original data packet is left unencrypted
* Only content of the data packet is encrypted
* Common in `Host-2-Site` VPN 

IPsec uses:
1. `Security Associations (SA)`
    * Define which types of hashing and encryption are used
2. `Internet Key Exchange (IKE)`
    * Secure exchange of cryptographic keys
3. Encryption and hashing algorithms
    * Algorithms that scramble data
4. Anti-Replay Protection
    * Network standards that stop hackers from `re-using data`

> IPsec authenticates data to ensure integrity, encrypts data to ensure confidentiality.