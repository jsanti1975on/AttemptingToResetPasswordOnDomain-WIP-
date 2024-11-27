Title explains all, My mentor set me up a domain and im assigned to change the password

I researched and 2 common methods are PowerShell and Using Active Directory Users and Computers (ADUC)

I decided to try powershell method first
![IMG_0548](https://github.com/user-attachments/assets/6a3d6b72-fe45-41ba-9987-769c55e66b14)


I typed the command "Import-Module ActiveDirectory" but however it was not loaded
![IMG_0549](https://github.com/user-attachments/assets/964405c4-bab9-4cdc-8a92-d984ed5e472e)


I moved on and put Set-ADAccount -Identity "username" -ResetPassword "newpassword". This was blocked off as well so powershell is No-Go
![IMG_0550](https://github.com/user-attachments/assets/19c914e9-3fd6-41e3-b6c6-ed24cb053e34)


From here it was most likely 2nd method so I manually went into my settings
![IMG_0551](https://github.com/user-attachments/assets/763e7958-ae7c-445f-af84-c7b61287895e)


After several attempts of changing up the password to the point that it was completely new I would often keep getting this error:
![IMG_0552](https://github.com/user-attachments/assets/bfae4677-5155-4a85-850b-2db9b81f6b3b)


After that my final method was by Using Active Directory Users and Computers (ADUC) and just by trying to run it windows could not find it. You can see I typed it correctly too.
![IMG_0554](https://github.com/user-attachments/assets/563c514d-50df-4d07-b56a-7884b4e64d4a)

