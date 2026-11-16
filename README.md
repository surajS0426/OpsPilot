# OpsPilot

## Priority rules

Every ticket gets a priority from P1 (most urgent) to P4, based on two questions:
who is affected (impact) and how badly their work is affected (urgency).

| Impact \ Urgency | Work stopped now | Work degraded | Can wait |
| --- | --- | --- | --- |
| Many users or a revenue system | P1 | P2 | P3 |
| One team | P2 | P3 | P3 |
| One person | P3 | P4 | P4 |

Categories: network, access, hardware, software, email, other.

One person: a single user.
One team: several users in the same team or office area.
Many users: more than one team, a whole site, or about 20 or more people, or any revenue system such as payments.

### Security Override

Security cases are prioritised by risk, but not by how many users are affected: 
-Suspected account compromise (password entered on a phishing page, unknown sign-in, MFA promps the user didn't trigger): at least P2, escalate to security on-call
-Phishing email reported but nobody clicked or entered details; P4, assign to the security queue for blocking and awareness
-Many users or a revenue system affected by a security incident: P1

### Environment definitions

Self-Service Portal: staff install and update approved software themselves
Device-Management tool: analysts can remotely push installs, updates and reinstalls
Software Catalogue: lists approved applications and versions
Identity admin console: service desk analysts can unlock accounts, reset passwords, re-register MFA devices and grant shared mailbox access. Changes to admin or finance-system permissions require the identity team.
Mail app and webmail: staff email on laptops and in the browser.
Cloud file-sync app: syncs staff files to cloud storage.