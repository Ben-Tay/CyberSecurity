## Snooping
> Hackers use snooping attacks to `intercept` data between devices

> Common in open-unsecured networks and can be difficult to trace

Attacks can reveal:
* Logins, credit card nos, IP etc

Examples:

`Eavesdropping (packet-sniffing)`
* Occurs on wireless, wired & phone connections
* A packet sniffer is a tool that intercepts everything transmitted on a network.
* Anything sent by a device on `unencrypted network` can be viewed by packet sniffer
* This allows hackers an opportunity to `intercept, alter, or delete data transmitted` between devices.

#### Safety mechanisms
* `Encrypted networks` make it such that packet sniffers can only see packet origin & destination, but not data inside it
* Staying off public wifi or using encryption with a
VPN or cellular connection helps prevent eavesdropping attacks.


`Man-In-The-Middle (On-Path attacks)`
* Form of eavesdropping
* Has a `victim, a receipt point, and an attacker`, where victim and receipt point are unaware of attacker listening in
* Can be:
    * `Physical:` attacker is physically near the victim,like the same public wifi network, or a network they set up themselves as a trap, by sniffing into that unencrypted network to `steal information`
    
    * `Logical`: attacker sends emails or texts with fake links that direct victims to sites that steal their data and install malware.

> Examples of MITM attacks: spoofing, hihacking, theft of browser cookies

`Replay`
* M-I-T-M attck that intercepts and retransmits data 
* Involves `trusted entities` -  users or websites that get an access token (or security key) after verifying that they are who they say they are.

> Hackers get access tokens by sniffing network traffic between trusted entities.
Once they find an access token, they can hijack the session and use the token to impersonate the `trusted entities`.

After Impersonation, the hacker can:
* Intercept and modify information
* Access private accounts as if they were the account holder

## Cross-Site Scripting (XSS)
> An attacker attaches malicious code onto a trusted site. The code activates when the site is loaded by a user.

`Reflected XSS`
* Malicious code is added to the end of a link’s URL 
* Eg: Link w/ malicious code in a `legitimate url`

How it works:
* When you click the link, it will still direct u to the website, but load malicious code in background to steal your info & send it to attacker

`Persisted XSS`
* Malicious code is embedded in unverified comments sections or forums.
* Malicious code runs every time the page is loaded by other users, delivering `your cookies and other data` to the attacker who can use it for `social engineering  or to break into your accounts`.

`Prevention Mechanisms`
* Validate inputs by creating rules for what people are allowed to enter in an editable field.
* Sanitize data by scanning for common malicious code and removing it.
* Set cookie rules to block data transfers to unfamiliar IP addresses, or to block JavaScript access.
* Configure a web application firewall (WAF) to stop cross-site scripting and other threats.

## SQL injection (SQLi)
* An attacker uses malicious SQL code to gain access to a website’s database.

Attackers can check vulnerability of a site to SQL injection through the following:
1. Log in with username or password with a `quotation mark` attached to it
2. If site returns syntax error, means that the `"` was recognized as code
3. This means that attacker can enter code commands into login field to bypass website's security to `access password protected info, download website database or even delete it`

`Prevention Mechanisms`
* Parameterize queries so the system only accepts predefined queries
* Store procedures so the system only accepts code that matches expected procedures.
* Use an allowlist so the system only accepts user content that matches expected values.
* Escape user input so the system won’t read user-added content as code

## Botnets
> Is a large collection of compromised, malware-infected computers `(zombie computers)`.

> Disclaimer: cryptominers are people who earn currency by solving difficult math problems

Allows hackers to: 
* access `hundreds/thousands of infected computers` remotely.
* perform large scale attacks 
* or computationally-intensive tasks - `crypto mining` which requires large amount of CPU power from other computers
    * Cryptomining software can be embedded into websites and can infect your computer giving attackers access to your computer.

## Denial of service
* Floods a network with so much traffic that it crashes
* DoS attack victims are typically high-profile,
like `government sites, banks, or social media sites.`

> Sometimes, DoS attacks are used to distract from other attacks happening at the same time.

`Common Dos Attacks`:
* Buffer Overflow - website gets more internet traffic than it can handle
* ICMP flood: when diagnostic pings are sent to every computer on a network to crash it `as each computer on network pings each other`
* SYN flood (TCP):
when a rapid series of incomplete connection requests floods a website until the server crashes

#### Distributed Denial of Service
> A Distributed Denial of Service (or DDoS) attack is when a DoS attack is made with a botnet.

DDoS attacks give attackers following advantages:
* Harder to identify attack origin to shut down
* More devastating as hundreds of computers used rather than `just one`