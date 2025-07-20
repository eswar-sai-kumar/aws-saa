# IAM (Identity and access management)

IAM is used to control who can access AWS resources and what they can do with them.

#### Users
People who use AWS accounts (like you and your team numbers)
#### Groups
Collections of users
#### Roles
Temporary access with specific permissions
#### Policies
Rules define what actions are allowed or denied (like read only access to S3)

## Creating User and adding to group

IAM → Users → Create User → User name → provide user access to AWS → I want to create an IAM user

![image](https://github.com/user-attachments/assets/2e4d5d3d-c66a-42f1-bc73-b1ee0efe6ef7)

password → Users must create new password at next sign in → next

![image](https://github.com/user-attachments/assets/0a413615-01cd-4b66-98db-1259d93b2007)

Add User → Create group

![image](https://github.com/user-attachments/assets/8d287965-4e8d-48bf-9d16-351f8a28c958)

User group name → AdministratorAccess(Permission policies) → Create user group

![image](https://github.com/user-attachments/assets/66fa23b6-73b6-4454-ac2d-0a37ee967513)

select admin1(forgot to select here) → next

![image](https://github.com/user-attachments/assets/3b919a27-44db-4bf7-bf76-2752279c045e)

Create 

![image](https://github.com/user-attachments/assets/553b1ef7-3ef1-45cb-a7c8-cd5adc1d142a)

## Creating acccess key

IAM → Users → Click on user you created → Security credentials

![image](https://github.com/user-attachments/assets/6e3cec70-bdc8-4b91-af6b-1ef2fe880563)

Create acccess key

![image](https://github.com/user-attachments/assets/be98fe2d-e16c-4f9c-a4cb-e31c0b6a6cc0)   

CLI

![image](https://github.com/user-attachments/assets/0179e7ad-c905-4087-a942-59a86759a0b6)

Confirm it → Next

![image](https://github.com/user-attachments/assets/e60976b1-0a7d-4014-a418-620ea0ee441e)

Create Access key

![image](https://github.com/user-attachments/assets/86985cb4-13c2-457a-a388-41c6b87f9ad2)

## ClousShell

Enter commands → Actions → download file → file path (/home/cloudshell-user/demo.txt) → download

![image](https://github.com/user-attachments/assets/e9deee9e-25a9-490a-b443-f745658cbd12)

demo.txt file 

![image](https://github.com/user-attachments/assets/5c315013-4af9-4b9a-a971-647b47375171)

## Creating Role

IAM → Roles → Create Role → AWS service → Use case(EC2) → next

![image](https://github.com/user-attachments/assets/67e19327-7021-4714-9eae-985d9af3d1a7)

Select permission policy(IAMReadOnlyAccess) → Next

![image](https://github.com/user-attachments/assets/c3162f79-0bed-47c7-91fc-e9c0e9857597)

Role name → Create Role

![image](https://github.com/user-attachments/assets/2edcdb27-e397-4cb3-8787-018f644b1f19)








