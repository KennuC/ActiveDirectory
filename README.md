# ProjectTemplate
# PROJECTNAME

## Objective
[Brief Objective - Remove this afterwards]

Peform Common task in Active Directory

### Skills Learned
[Bullet Points - Remove this afterwards]

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
[Bullet Points - Remove this afterwards]

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps
drag & drop screenshots here or use imgur and reference them using imgsrc

Every screenshot should have some text explaining what the screenshot is about.

Example below.

*Ref 1: Network Diagram*
## Links to skip to sections

## Create Active Directory Users from CSV with PowerShell

Using Excel to create random users under a simple template

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/f6380f1d-d2fa-4c64-a9fa-62136d179e1a)

Finding the distinguishedName to fill the organisation unit (OU) on the Excel

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/c5f4ae92-4855-495b-9ea8-b2cfc226ad27)

Placing the value in the fields under OU

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/c0ea2cff-699b-4105-923c-bd5014c48474)

Saving as CSV

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/e674ac79-cdee-4cb1-86fa-5d6c1c57a55e)

Importing CSV in Powershell to see if the script is readable.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/b8670265-81c9-4d20-b9af-ee9f52d22f78)

Preparing the Powershell script

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/608aa8cc-02ed-413b-b82d-08bc561d559c)

Running the AddUserScript Powershell script

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/dab8a37a-0724-4ab3-9839-4a0a29358a5c)

Can see now that under HR, users are successfully created.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/25b94d36-293e-4800-9ccd-a51d418af0fe)

Repeating step for IT

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/08e8d1f4-d254-44c1-bc85-cac2c24708c9)

## Common Active Directory Tasks

### Finding users on Active Directory

Under the forest, selecting find.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/75fcca63-9730-40e8-91fd-f22e865cb49c)

Find: Users, Contacts, and Groups In: Entire Directory, for example searching for Ethan.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/a090164f-f2e8-40fc-8deb-21cdcbb873e0)

### Password Reset

Lets say if Ethan's password needs to be resetted, showing options and selecting reset password and then giving Ethan a temporary password for them to change password on next logon

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/cc46be29-4504-461a-8786-83cd87072b64)
![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/f48f2285-2d47-4e3a-81fa-de8ef73b3134)

