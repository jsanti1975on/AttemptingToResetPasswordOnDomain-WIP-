Title explains all, My mentor set me up a domain and im assigned to change the password

I researched and 2 common methods are PowerShell and Using Active Directory Users and Computers (ADUC)

I decided to try powershell method first
![IMG_0548](https://github.com/user-attachments/assets/2a68d9ca-3c82-49fd-b231-2fa0218e0de7)



I typed the command "Import-Module ActiveDirectory" but however it was not loaded
![IMG_0549](https://github.com/user-attachments/assets/964405c4-bab9-4cdc-8a92-d984ed5e472e)


I moved on and put Set-ADAccount -Identity "username" -ResetPassword "newpassword". This was blocked off as well so powershell is No-Go
![IMG_0550](https://github.com/user-attachments/assets/b51cf63f-6379-401b-adee-9ad1c6a56eff)



From here it was most likely 2nd method so I manually went into my settings
![IMG_0551](https://github.com/user-attachments/assets/b2dce64f-4bb8-4e97-b2ae-4e586a457bd0)



After several attempts of changing up the password to the point that it was completely new I would often keep getting this error:
![IMG_0552](https://github.com/user-attachments/assets/37672f9d-a8a0-4221-8ebb-bfde1085b517)



After that my final method was by Using Active Directory Users and Computers (ADUC) and just by trying to run it windows could not find it. You can see I typed it correctly too.
![IMG_0554](https://github.com/user-attachments/assets/28a727ca-585f-4532-acfe-d1c8ca82afcb)

