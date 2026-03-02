# 365-Tenant
This is a 365 tenant to study for the SC300 exam
PART 1
Created Office 365 E5 free trial tenant
<img width="975" height="490" alt="image" src="https://github.com/user-attachments/assets/6968e90b-5fa8-4f0a-9fb2-bd08749cd450" />
Started Free Trial for Microsoft 365 E5 License
<img width="975" height="491" alt="image" src="https://github.com/user-attachments/assets/139814f7-c561-4e61-acff-ede9ab231483" />
Created a series of User accounts 
<img width="2556" height="1093" alt="image" src="https://github.com/user-attachments/assets/9eb43bb1-f77f-4cd3-bc07-3a75ba15693c" />
Created a series of Security Groups. Each group is tied to their specific role within the company. For example, HelpDesk1 is assigned to the Help Desk Group.
<img width="2552" height="862" alt="image" src="https://github.com/user-attachments/assets/915237ac-501d-40ef-97b3-1097d58837f9" />
Each user account has a specific role. This was just for documentation purposes, we will later remove these roles and assign the roles and apply them to security groups for IT hygine. As you can see from the screenshot below, the Help Desk1 user account has been assigned an active Helpdesk Administrator Role. The idea here is the concept of least privilege, only giving a user the access that is necessary for them to do their job duties. 
<img width="2556" height="778" alt="image" src="https://github.com/user-attachments/assets/cccacd52-72f6-424a-950f-fa6229245d36" />
Now I have removed the roles for specific user accounts, and applied them to the security groups. This allows for easier workflows when onboarding our new employees, simply adding them to the proper group will provide them the access they need to perform their job duties. User Accounts, Help Desk1 & Help Desk2 have been added as members of the Help Desk security group. The Help Desk security group has permanent Active Help Desk Admin and User Admin roles assign to them. 
<img width="2555" height="554" alt="image" src="https://github.com/user-attachments/assets/3c82fd26-a88b-4486-b637-1c2df8be6892" />
<img width="2556" height="481" alt="image" src="https://github.com/user-attachments/assets/21b4b7a5-8590-47e3-b9a8-adb7eb13b9f6" />
Without cluttering this with screenshots, the following groups have these permanent role assignments:
-Vince Craft - User account that has Global Admin role
-Break Glass - User account that has Global Admin role
-HR - Sharepoint Administrator
-IAM - Authentication Policy Administrator, Groups Administrator, Privileged Authentication Administrator, License Administrator, Security Reader, Privileged Role Administrator, User Administrator, Conditional Access Administrator, Authentication Administrator
-Security Team - Security Administrator
-Teams Admin - Teams Administrator
-The point of this is separation of duties, only giving the memebers of these security groups the access they need to perform their job duties. As you can see by the screenshot below, the user account Help Desk1 now has active role assignments that have been applied through GROUP membership.
<img width="2553" height="446" alt="image" src="https://github.com/user-attachments/assets/ed3bf0f6-125e-4e08-a631-2336850c4256" />
PART 2
Enabled guest self-service sign up via user flows
<img width="2580" height="1040" alt="image" src="https://github.com/user-attachments/assets/4fc2c146-defa-4d53-927e-f6f49a6b5cc1" />
Ensured that Email one-time passcode was configured for authentication in External Identities 
<img width="2555" height="684" alt="image" src="https://github.com/user-attachments/assets/0559b433-9200-4aef-96cf-09406b0d1d96" />
Further configured the external collaboration settings. Guest user access is restricted to properties and memberships of their own directory objects. Guest invite settings are restricted to member users and users assigned to specific admin roles can invite guest users including guests with member permissions. Collaboration restrictions are set to allow invitations to be sent to any domain.
<img width="2552" height="1101" alt="image" src="https://github.com/user-attachments/assets/151e695a-b007-4309-83fd-694c3ecffa34" />
Enabled MFA for all user accounts 
<img width="2549" height="924" alt="image" src="https://github.com/user-attachments/assets/fd6abb29-5110-4fe2-9b99-0f04ba1c16f2" />
Created conditional access policy to require MFA (break glass account excluded)
<img width="2556" height="1061" alt="image" src="https://github.com/user-attachments/assets/1e51ca1c-17fd-4577-b726-01bf7af5b03d" />
Configuring SSPR // 
First, I created a group SSPR Testers and added all user accounts
<img width="2555" height="904" alt="image" src="https://github.com/user-attachments/assets/3fead3fd-8078-4022-8741-b12a16cb4377" />
Enabled SSPR and added the SSPR Testers group
<img width="2546" height="725" alt="image" src="https://github.com/user-attachments/assets/ebb14af7-2767-4c11-a4e1-b04da553de69" />
Confirmed that 1 authentication method is required to reset 
<img width="2556" height="648" alt="image" src="https://github.com/user-attachments/assets/fe1b3fa2-6c13-4c24-b76c-959f85004bee" />
