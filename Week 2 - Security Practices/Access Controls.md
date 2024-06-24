## The 3 A's
> 3 processes involved in logging into a network or account

`Access Control` 
* Limiting/granting access to different areas based on user status
* Prevents unauthorized viewing, modification, or copying of data.
* IT staff use AC to restrict:
    1. What users can do
    2. Which resources they have access to
    3. What functions they are allowed to perform

#### Rule of Least Privilege
* Access is granted only when a user needs it to fulfill their role

> Role-based access control (or RBAC) follows a company’s org chart.
* Different customer and employee roles are set up as groups on a network,and then those groups are granted certain permissions.
* When a new user joins the network, they are assigned to the group `that fits their role` and assigned the `least permissions` to do their job

`Authorization` – giving permission to access a computer, network, app, or account or do an action
* Access control must be set up before authorization is granted `to maintain data security`
* Authorization must be set up for your user account before you’re able to log in.
* Once you are authorized, you can then use authentication to log in.

`Authentication` – confirming the identity of a user 
* Involves 2 steps
* Login Information + Identity confirmation = Authentication
* Authentication factors mentioned in previous file
* Authentication Methods: (SFA, 2FA, MFA, SSO), also covered in previous file

> Access control sets boundaries, authorization gives access,and authentication confirms identity.

Need to find the balance between the 3 A's

`Authorization vs Access Control`
* Strictly applying role-based permissions groups won’t secure data if those groups all have the same authorization levels.

`Authentication vs Access Control`
* Using strong passwords and MFA won’t secure data if all groups have the same permissions.

`Authentication vs Authorization`
* Using strong passwords and MFA won’t secure data if all users are assigned to the same group.

> Best practice should require strong authentication, strong authorization, and strong access control.

## Digital Accounting
> Digital accounting is used in troubleshooting, security analysis, forensics, and hacking.

`Audit logs to show:`
* Who did what
* How the system responded

`Tracking`: 
Websites can track your OS, browser version, installed extensions, screen resolution,
installed fonts, time zone, language, and how long you spent on a site and what you did there.

`Cookie`:
* A cookie is code used to track, personalize, and save information about your browsing session.
* Can also be used to ban a user from a website if they violated any terms and conditions

`Browsing history`:
* is a list of recently visited websites.
* Anyone with access to your device can see what sites you visited.
* Attackers use browsing history to learn where they might impersonate their victims, and companies use it to see which sites you go to on your work computer.

## Non-Repudiation
* Can't deny being in a specific location.
It guarantees that a message sent between two parties is genuine.

Real life examples
* `Videos` - Clear recordings of a person entering, leaving, or occupying a spac
* `Biometrics` - fingerprint or iris scans can confirm whether a person physically accessed a device, network, or area.
* `Signature`- When a signature is used in conjunction with a hardware token,
it becomes a digital signature. This authenticates the signer.
* `Receipt` - A digital receipt proves that a message was sent from one party to another.
