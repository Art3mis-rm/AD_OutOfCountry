# AD_OutOfCountry
This script will retrieve the list of all users from the AD who are logging in from outside the USA. If scheduled to run weekly or monthly, this script will give you a list of new users who are logging in from outside the USA

----------------------------------------------------------------------------------------
Usage:
----------------------------------------------------------------------------------------
1. Download the bat file: 'AD_OutOfCountry.bat'
2. Create a folder (OutOfCountry-Reports) and move the bat file to this folder 
2. Open Powershell with admin access
3. In Poweshell, Navigate to the folder (OutOfCountry-Reports) where 'AD_OutOfCountry' is saved
4. To create two new csv files, run the following two commands in the powershell:

  New-Item ./Adusers_Country_Total.csv -ItemType File

  New-Item ./Adusers_Country_New.csv -ItemType File

5. Create a new folder and name it as bin (..\Country_Alerts\bin)
6. In powershell, navigate to folder (bin) and run the following command:

New-Item ./Adusers_Country_Old.csv -ItemType File

7. Once all the above steps are executed, double click on the batch file (AD_OutOfCountry)

Note: The names of the files and folder should NOT be changed

----------------------------------------------------------------------------------------
Additional Information
----------------------------------------------------------------------------------------

Adusers_Country_Total = COMPLETE list of employees logging in from outside US
Adusers_Country_New = List of NEW users who are logging in from outside US (Compares with Adusers_Country_Total and outputs new entries)

United Kingdom : GB
Switzerland : CH


