# EXAMPLES OF ROOT USER
1. They are usually identified as root and are superuser with unlimited power.
## REGULAR USER
JANE,JAMES. these are the employees with limited power and are people writing codes everyday,browsing files etc.
each user has a username, a home directory and limited permissions.
### SYSTEM USER
They are like invisible workers and not real people. don't need a home directory or password.

### MISSION 1
For /etc/passwd: it shows every user, the system,root and regular user.
for /etc/shadow : store all the passwords in the system and therefore access was denied to me when  i tried  the cat /etc/shadow command.
for /etc/group: stores all information about the UID and the GID.

#### PHASE 2
Username: ada,femi and kosi
Descriptive role: Ada-Developer, Femi-Support Specialist,Kosi-Temporary Contractor
UID:Ada-1006, Femi-1007, Kosi-1008
Primary GID: Ada-1006, Femi-1007, Kosi-1008
Home directory: Ada-/home/Ada, Femi-/home/Femi, Kosi-/home/Kosi
Default shell: Ada-/bin/sh, Femi-/bin/sh, Kosi-/bin/sh
Expected account type:Ada-regular account, Femi-regular and Kosi-temporary account.
Secondary GID:
uid=1006(Ada) gid=1006(Ada) groups=1006(Ada),1008(Developers),
uid=1008(tobi) gid=1009(tobi) groups=1009(tobi)1008(Developers),
 uid=1007(Femi) gid=1007(Femi) groups=1007(Femi),1011(Support),
uid=1009(Nneka) gid=1010(Nneka) groups=1010(Nneka),1012(Auditor)

<TABLE>
<tr><th>User</th><th>Primary group</th><th>Supplementary group before<th><th>supplementary group after
</th><th>Reason for access</th></tr>
<tr><td>Ada</td><td>1006</td><td>1006, Developers-1008 </td><td>Projectx-1013 </td><td>Developers for projectx</td></tr>
<tr><td>Femi</td><td>1007</td><td>1007, Support-1011</td><td> N/A</td><td>Support Specialist</td></trf>
<tr><td>Nneka</td><td>1009</td><td>1010, Auditor-1012</td><td>Projectx-1013</td><td>Auditor for projectx</td></tr>
<tr><td>tobi</td><td>1008</td><td>1009, Developers-1008</td><td>Projectx-1013</td><td>Project Leader</td></tr>



