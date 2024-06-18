# Active Directory

## Objective

The objective of this project is to gain proficiency in managing Active Directory Domain Services through hands-on, practical tasks. 

### Skills Learned
- [Create Active Directory Users from CSV with PowerShell](#create-active-directory-users-from-csv-with-powershell)
- [Finding Users on Active Directory](#finding-users-on-active-directory)
- [Password Reset](#password-reset)
- [Enable Recycle Bin](#enable-recycle-bin)
- [Using CMD to find user information](#using-cmd-to-find-user-information)
- [Installing RSAT Tools on Windows10 Machine](#installing-rsat-tools-on-windows10-machine)

### Tools Used
- **VirtualBox**: For setting up virtual machines to create a controlled lab environment.
- **Active Directory Domain Services**: Manage users under domain.
- **Excel**: To create a table of users to be exported to CSV file.
- **PowerShell**: For script execution to add users using a CSV file.

## Create Active Directory Users from CSV with PowerShell

1. Using Excel to create a table of random users under a simple template.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/f6380f1d-d2fa-4c64-a9fa-62136d179e1a)

*Ref 1. User Spreadsheet*

2. Finding the `distinguishedName` under OU `Properties`, `Attribute Editor`. Using this value to fill the organisation unit (OU) on the Excel

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/c5f4ae92-4855-495b-9ea8-b2cfc226ad27)

*Ref 2. Obtaining value*

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/c0ea2cff-699b-4105-923c-bd5014c48474)

*Ref 3. Placing the value in the fields under OU*

3. Saving as CSV to store information in plain text form to be used in PowerShell

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/e674ac79-cdee-4cb1-86fa-5d6c1c57a55e)

*Ref 4. Saving as CSV*

4. Import the CSV file into Powershell to verify the script is readable.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/b8670265-81c9-4d20-b9af-ee9f52d22f78)

*Ref 5. Importing CSV in Powershell*

5. Preparing a Powershell script to use the saved CSV file to automatically create users in Active Directory.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/608aa8cc-02ed-413b-b82d-08bc561d559c)

*Ref 6. Preparing Powershell script*

6. Running the prepared Powershell script shows that each user listed in the CSV file is created.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/dab8a37a-0724-4ab3-9839-4a0a29358a5c)

*Ref 7. Running Powershell script*

7. Checking the Active Directory, we can see now that under HR, users are successfully created.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/25b94d36-293e-4800-9ccd-a51d418af0fe)

*Ref 8. HR User creation verification*

8. Now repeat the steps for IT.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/08e8d1f4-d254-44c1-bc85-cac2c24708c9)
*Ref 9. IT User creation verification*

## Finding users on Active Directory

Under the forest, select `find`.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/75fcca63-9730-40e8-91fd-f22e865cb49c)

*Ref 10. Find option*

Find: `Users, Contacts, and Groups` In: `Entire Directory`, for example searching for `Ethan`.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/a090164f-f2e8-40fc-8deb-21cdcbb873e0)

*Ref 11. Find user example*

## Password Reset

Let's say Ethan's password needs to be reset, in options, select `Reset Password` and then give Ethan a temporary password for them to change the password on the next login.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/cc46be29-4504-461a-8786-83cd87072b64)

*Ref 12. Reset Password option*

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/f48f2285-2d47-4e3a-81fa-de8ef73b3134)

*Ref 13. Reset Password option (Cont.)*

## Enable Recycle Bin

In the Start bar, under `Windows Administrative Tools`, select `Active Directory Administrative Center`.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/22896780-f19e-4222-b4cf-437719f50e50)

*Ref 14. Windows Start bar*

Under DC `kennu(local)`, enable the recycle bin.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/d4b278f9-e6f9-42fd-a6f1-27d7fa81b73c)

*Ref 15. Active Directory Administrative Center*

## Using CMD to find user information

In the command prompt, typing in `net user <username> /domain` will show details of the user like password details, local groups and global groups.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/c57dd04c-e84c-4289-8804-7eb8e4d3b29c)

*Ref 16. User information in CMD*

## Installing RSAT Tools on Windows10 Machine

In optional feature, adding an optional feature, select relevant RSAT tools to install. Installing RSAT tools on a Windows 10 machine allows administrators to manage Active Directory and other server roles remotely, providing convenience and reducing the need to directly access the server.

![image](https://github.com/KennuC/ActiveDirectory/assets/131323586/470ab3b1-61a6-4b8d-925b-1b1254205abf)

*Ref 17. Adding optional features*
