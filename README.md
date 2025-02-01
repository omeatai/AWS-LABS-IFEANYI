# AWS-LABS-IFEANYI
### by Ifeanyi Omeata

#### Join me as I complete 300+ Labs and Projects in the AWS Cloud. Follow my Youtube channel at https://www.youtube.com/@omeatai

<details>
  <summary>Project 1 - Create an IAM User and Group in AWS</summary>

  ###

  <a href="https://youtu.be/svUj_aHjNVk" target="_blank"><img src="https://github.com/user-attachments/assets/d0953b7c-1ff4-4445-bc63-f7f014832cf7" width="720" height="400" /></a>

  ### 1. Open IAM Console
  - [ ] **Go to the AWS Management Console.**
  - [ ] **Enter "IAM" in the search bar and go to the IAM console.**
  - [ ] **Notice the IAM service is global and doesn't require region selection.**

  ### 2. Viewing Current Users
  - [ ] **On the left-hand side, click on "Users" to view the current user list.**

  ### 3. Create a New IAM User and Set Password
  - [ ] **Click on "Create user."**
  - [ ] **Enter a username (e.g., admin).**
  - [ ] **Select "Provide user access to the AWS Management Console."**
  - [ ] **Choose "I want to Create an IAM user" option.**
  - [ ] **Choose "Custom password" and enter your password.**
  - [ ] **Uncheck "Users must create a new password at next sign-in.”**
  - [ ] **Click "Next".**

  ### 4. Create a User Group and Assign Permissions
  - [ ] **Choose "Add user to group."**
  - [ ] **Click "Create group."**
  - [ ] **Name the group (e.g., administration).**
  - [ ] **Attach "AdministratorAccess" policy to the group.**
  - [ ] **Click "Create user group".**
  - [ ] **Add the user to the newly created admin group by selecting the group.**
  - [ ] **Click "Next".**

  ### 5. Review and Create User
  - [ ] **Review the settings: username, permissions, groups, etc.**
  - [ ] **Optionally, add tags (e.g., department: engineering).**
  - [ ] **Click "Create user."**

  ### 6. Verify User and Group Setup
  - [ ] **Optionally, download the CSV file for sign-in credentials.**
  - [ ] **View the user list to ensure the user is created.**
  - [ ] **Verify the user belongs to the "administration" group.**
  - [ ] **Check the "administration" group to confirm "AdministratorAccess" policy is attached.**

  ### 7. Create an Account Alias (Optional)
  - [ ] **Go to your AWS IAM Dashboard.**
  - [ ] **Create an account alias (e.g., aws-adminaccess-v2).**

  ### 8. Sign in with IAM User
  - [ ] **Open a new private browser window.**
  - [ ] **Use the IAM sign-in URL.**
  - [ ] **Enter account alias or account ID, and IAM username (e.g., admin).**
  - [ ] **Enter the IAM user password to log in.**
  - [ ] **Check the top right to ensure you're signed in as the IAM user.**

</details>

<details>
  <summary>Project 2 - Create IAM Policies</summary>

  ###

  <a href="https://youtu.be/SJsFRshZMo0" target="_blank"><img src="https://github.com/user-attachments/assets/1d9813f0-3779-4fb3-bde0-5d769a454c5b" width="720" height="400" /></a>
 
  ### 1. Inspect IAM Policies and Explore Read-Only Policy
  - [ ] **On the left-hand side, click "Policies."**
  - [ ] **Look at the "AdministratorAccess" policy details.**
  - [ ] **Review the summary and JSON format of the policy.**
  - [ ] **Look at the "IAMReadOnlyAccess" policy details.**
  - [ ] **Inspect the API calls allowed and view the JSON representation.**

  ### 2. Create a Custom Policy
  - [ ] **Click "Create policy."**
  - [ ] **Use the "Visual editor" or “JSON” to select actions like "ListUsers" and "GetUser."**
  - [ ] **Authorize on "All resources."**
  - [ ] **Name the policy (e.g., MyNewIAMPermissions) and create it.**
  - [ ] **Inspect the JSON document of the newly created policy.**

</details>

