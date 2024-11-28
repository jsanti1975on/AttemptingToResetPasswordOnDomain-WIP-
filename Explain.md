# Title Explains All: Changing the Password on a Domain

## Overview
My mentor set me up with a domain, and I was assigned the task of changing the password. After researching, I found two common methods for accomplishing this:

1. Using **PowerShell**
2. Using **Active Directory Users and Computers (ADUC)**

I decided to try the **PowerShell** method first.

---

## Attempt 1: Using PowerShell

### PowerShell Command
I typed the following command:
```powershell
Import-Module ActiveDirectory
```
**Outcome**:  
The module did not load.

#### Import Module Error
```plaintext
The term 'Import-Module ActiveDirectory' is not recognized as the name of a cmdlet, function, script file, or operable program.
```

---

### Second PowerShell Command
Next, I tried the following command:
```powershell
Set-ADAccount -Identity "username" -ResetPassword "newpassword"
```
**Outcome**:  
This command was also blocked. At this point, I realized PowerShell wasn't a viable option.

#### Set-ADAccount Error
```plaintext
The term 'Set-ADAccount' is not recognized as the name of a cmdlet, function, script file, or operable program.
```

---

## Attempt 2: Manual Navigation

I manually navigated through the settings on my system. Despite trying several different password combinations, including completely new ones, I kept encountering this error:

#### Password Change Error
```plaintext
The password does not meet the complexity requirements of the domain policy.
```

---

## Attempt 3: Using Active Directory Users and Computers (ADUC)

As a final attempt, I tried using the **Active Directory Users and Computers (ADUC)** tool. However, when I searched for it, Windows was unable to locate it. I double-checked that I had typed the name correctly.

#### ADUC Not Found
```plaintext
Windows cannot find 'dsa.msc'. Make sure you typed the name correctly, and then try again.
```

---

## Conclusion
After multiple attempts to change the password using PowerShell, manual navigation, and ADUC, I encountered various obstacles:

1. **PowerShell**: The required commands or modules were unavailable.
2. **Manual Navigation**: Domain policies prevented the password from being accepted.
3. **ADUC**: The tool could not be located on the system.

This experience highlighted the importance of verifying system configurations and permissions before proceeding with administrative tasks.
