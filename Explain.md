Title explains all, My mentor set me up a domain and im assigned to change the password

I researched and 2 common methods are PowerShell and Using Active Directory Users and Computers (ADUC)

I decided to try powershell method first
![IMG_0548](https://github.com/user-attachments/assets/672e4d2f-71e5-4164-aacf-452d050748eb)

I typed the command "Import-Module ActiveDirectory" but however it was not loaded
![IMG_0549](https://github.com/user-attachments/assets/8f508188-4a9a-4dba-80b7-e957abb2e28d)

I moved on and put Set-ADAccount -Identity "username" -ResetPassword "newpassword". This was blocked off as well so powershell is No-Go
![IMG_0550](https://github.com/user-attachments/assets/4f55863d-03a4-421c-8609-aae2a6e4a8d3)

From here it was most likely 2nd method so I manually went into my settings
![IMG_0551](https://github.com/user-attachments/assets/36d1adcc-192a-43d6-a48f-a302dc4a81fa)

After several attempts of changing up the password to the point that it was completely new I would often keep getting this error:
![IMG_0552](https://github.com/user-attachments/assets/4d8eb23b-460e-405b-be50-b8bd10d75113)

After that my final method was by Using Active Directory Users and Computers (ADUC) and just by trying to run it windows could not find it. You can see I typed it correctly too.
![IMG_0554](https://github.com/user-attachments/assets/850b9021-4d60-4a8c-85a2-d33688224f64)
