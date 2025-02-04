# AWS-LABS
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

<details>
  <summary>Project 3 - Install AWS CLI on Windows PC</summary>

  ###

  <a href="https://youtu.be/h5HW1z7BS9M" target="_blank"><img src="https://github.com/user-attachments/assets/e89b6c6f-a2c1-4988-b50b-7e0e5eba1883" width="720" height="400" /></a>

  ### 1. Search for AWS CLI Installation
  - [ ] **Open a web browser.**
  - [ ] **Search for "aws CLI install windows" using a search engine like Google.**

  ### 2. Download and Run AWS CLI Version 2 Installer
  - [ ] **Find the official AWS CLI Version 2 download link for Windows.**
  - [ ] **Scroll to the "AWS CLI install and update instructions" section.**
  - [ ] **Select the drop-down for Windows option.**
  - [ ] **Click the link to download the MSI installer for AWS CLI Version 2.**
  - [ ] **Locate the downloaded MSI installer file.**
  - [ ] **Double-click the file to run the installer.**
  - [ ] **Click "Next" to proceed with the installation.**
  - [ ] **Accept the license agreement terms.**
  - [ ] **Click "Next" and then click "Install."**
  - [ ] **Allow any necessary permissions for the installer to proceed.**
  - [ ] **Wait for the installation to finish.**
  - [ ] **Click "Finish" to complete the setup.**

  ### 3. Verify AWS CLI Installation
  - [ ] **Open "Command Prompt" on Windows.**
  - [ ] **Type `aws --version` and press Enter.**
  - [ ] **Check for output that starts with "aws-cli/2" followed by the Python version and Windows details.**
  - [ ] **Confirm that AWS CLI version 2 is installed and working correctly.**

</details>

<details>
  <summary>Project 4 - Create CLI Access Keys</summary>

  ###

  <a href="https://youtu.be/YFVP_o9Z_1k" target="_blank"><img src="https://github.com/user-attachments/assets/a3a7667a-22db-4c9a-b64e-9f5f850e24e5" width="720" height="400" /></a>

  ### 1. Navigate to Security Credentials
  - [ ] **Open the IAM Console.**
  - [ ] **Click on your username (e.g., admin).**
  - [ ] **Go to the "Security credentials" section.**
  - [ ] **Scroll down to the "Access keys" section.**
  - [ ] **Click "Create access key."**

  ### 2. Create an Access Key
  - [ ] **Choose the purpose for the access key, such as CLI.**
  - [ ] **Acknowledge AWS's recommendations regarding alternative methods.**
  - [ ] **Check "I understand the above recommendation" to proceed.**
  - [ ] **Generate the access key and secret access key.**
  - [ ] **Save the access key and secret access key immediately as this is the only time they will be visible.**

  ### 3. Configure AWS CLI
  - [ ] **Open Command Prompt on Windows.**
  - [ ] **Run the command `aws configure`.**
  - [ ] **Enter the access key ID when prompted.**
  - [ ] **Enter the secret access key when prompted.**
  - [ ] **Set the default region (e.g., us-east-2).**
  - [ ] **Set the default output format (press Enter to skip or choose format).**

  ### 4. Verify AWS CLI Configuration
  - [ ] **Execute a test command like `aws iam list-users`.**
  - [ ] **Confirm the output matches your IAM console, showing user details.**

  ### 5. Modify User Permissions
  - [ ] **Use your root account to remove the user (e.g., admin) from the "administration" group.**
  - [ ] **Verify the user now has no permissions.**

  ### 6. Test Permissions with CLI
  - [ ] **Run `aws iam list-users` in CLI.**
  - [ ] **Confirm that no response is returned due to lack of permissions.**

  ### 7. Re-add User to Administration Group
  - [ ] **Go back to "User groups."**
  - [ ] **Add the user (e.g., admin) back into the "admin" group to restore permissions.**
  - [ ] **Verify that the user permissions have been successfully restored.**

</details>

<details>
  <summary>Project 5 - Create IAM Roles for EC2 Access</summary>

  ###

  <a href="https://youtu.be/Ek2348dchLI" target="_blank"><img src="https://github.com/user-attachments/assets/5ccf2c8a-ccb7-4013-8852-bf981045da49" width="720" height="400" /></a>
 
  ### 1. Open the Roles Section
  - [ ] Navigate to the IAM Console.
  - [ ] On the left-hand side, click on "Roles."
  - [ ] Observe any pre-existing roles in your account.

  ### 2. Create and Choose a New Role
  - [ ] Click on "Create role."
  - [ ] Select "AWS service" as the trust entity type.
  - [ ] Choose the service for this role, such as EC2.
  - [ ] Identify the use case for the selected service, e.g., "EC2."

  ### 3. Attach Permissions Policy and Role Name
  - [ ] Attach a permissions policy to the role.
  - [ ] Select "IAMReadOnlyAccess" to allow EC2 instances to read from IAM.
  - [ ] Review the selected permissions for the role.
  - [ ] Enter a role name, e.g., "DemoRoleForEC2."
  - [ ] Confirm the trusted entity is EC2, indicating that EC2 instances can assume this role.

  ### 4. Create the Role
  - [ ] Verify all settings and click "Create role."
  - [ ] Ensure the newly created role appears in the role list.
  - [ ] Check role details to confirm correct permissions are attached.

</details>

<details>
  <summary>Project 6 - Generate Credentials Report and Use IAM Last Accessed</summary>

  ###

  <a href="https://youtu.be/T0fCqBq8QOI" target="_blank"><img src="https://github.com/user-attachments/assets/b6007b82-fcd1-49f0-ac0e-7a7c27af9025" width="720" height="400" /></a>

  ### 1. Generate a Credentials Report
  - [ ] Navigate to the **IAM Console**.
  - [ ] On the left-hand menu, click on **"Credential report"**.
  - [ ] Click **"Download credential report"** to generate a CSV file.
  - [ ] Open the downloaded CSV file.

  ### 2. Open and Review CSV file  
  - [ ] Review the following details for user accounts:
    - User creation date.
    - Password status (enabled or not).
    - Last password usage and change dates.
    - MFA (Multi-Factor Authentication) status.
    - Access keys status (created, rotated, last used).
    - Password rotation policy (if enabled).
  - [ ] Use the report to identify security concerns, such as:
    - Users who haven’t changed their passwords recently.
    - Accounts without MFA enabled.
    - Unused or outdated access keys.
  - [ ] Use the **Credentials Report** for periodic security audits.

  ### 3. Access IAM Last Accessed
  - [ ] Go back to the **IAM Console** and select a specific user (e.g., "ifeanyi").
  - [ ] On the user’s detail page, click on **"Last Accessed"** on the right-hand side.
  - [ ] Check the list of AWS services accessed by the user, including:
    - Services that were accessed and the last access date.
    - Services not accessed by the user.
  - [ ] Identify which permissions granted access to specific services (e.g., Amazon EC2 via AdministratorAccess policy).
  - [ ] Use the data from Access Advisor to determine if the user requires access to all granted services.
  - [ ] Consider removing unnecessary permissions for enhanced security.
  - [ ] Use **Access Advisor** to perform a granular review of user permissions and optimize access policies.

</details>

<details>

<summary>Project 7 - Lunch an EC2 Instance with a Web Server </summary>

 ###

<a href="https://youtu.be/GyQrcAfVxBE" target="_blank"><img src="https://github.com/user-attachments/assets/43b8e9a0-3034-4412-91ae-cfaa486ec932" width="720" height="400" /></a>

### 1. Launch an Instance
- [ ] Go to **EC2 Console** → Click **Instances** → Select **Launch Instances**.
- [ ] Add Name: Enter **"My First VM Instance"**.
- [ ] Select **Amazon Linux (free tier eligible)**.
- [ ] Use **t2.micro instance type** (free tier eligible for 750 hours/month).

### 2. Set Up a Key Pair
- [ ] Create a new key pair (e.g., **EC2 key**).
- [ ] Download the **.pem file** (essential for SSH access).

### 3. Configure Network Security and Storage Configuration
- [ ] Automatically assign a **Public IP Address**.
- [ ] Set up Security Groups:
  - [ ] Allow **SSH (port 22)**.
  - [ ] Allow **HTTP (port 80)**.
- [ ] Use the default **8 GB gp2 root volume** (free tier allows up to 30 GB).

### 4. Add User Data and Launch the Instance
- [ ] Include a script to:
  - [ ] Update system packages.
  - [ ] Install the **HTTPD web server**.
  - [ ] Deploy a **"Hello World"** HTML page.
  ```bash
    #!/bin/bash
    # Executed when instance is first launched, to automate the setup and configuration of instance.
    # Update all the packages on the system to their latest versions
    yum update -y
    # install Apache HTTP server (httpd - Linux 2 version)
    yum install -y httpd
    # starts the Apache HTTP server
    systemctl start httpd
    # Enable auto server boot
    systemctl enable httpd
    # Hello World HTTP Page
    echo "<h1>Hello World from Private Host $(hostname -f)</h1>" > /var/www/html/index.html
    echo "<br/><br/><p>Created by Ifeanyi Omeata</p>" >> /var/www/html/index.html
  ```
- [ ] Review all settings.
- [ ] Click **Launch Instance**.

### 5. Testing and Managing the Instance
- [ ] Check the **Instance Name, ID, and State**.
- [ ] Copy the **Public IPv4 Address**.
- [ ] Open it in a browser using **http://<Public_IP>**.
  - [ ] Ensure the URL uses **HTTP**, not HTTPS.
- [ ] Stop Instance: Pause the instance to save costs.
- [ ] Review attached **Storage Volumes** and **Security Groups**.

</details>

<details> 
  <summary>Project 8 - Lunch an EC2 Instance with a Web Server on VPC </summary>

 ###
 
<a href="https://youtu.be/TmDIpZ9ynuk" target="_blank"><img src="https://github.com/user-attachments/assets/192d830e-5143-4083-ae73-706cb4dfb789" width="720" height="400" /></a>

### Task 1: Provision Default VPC
- [ ] Ensure the default AWS Region is set to **US East (N. Virginia) us-east-1**.
- [ ] Navigate to **VPC** either through:
  - [ ] Clicking on the **Services** menu → VPC.
  - [ ] Or directly via [Amazon VPC console](https://console.aws.amazon.com/vpc/).
- [ ] Delete the default VPC:
  - [ ] Select **Your VPCs** from the navigation pane.
  - [ ] Choose the **VPC** with "yes" in the default VPC column.
  - [ ] Click on the **Actions** button → **Delete VPC**.
  - [ ] Check **I acknowledge that I want to delete my default VPC**.
  - [ ] Confirm by typing "delete default VPC" and click on **Delete**.
- [ ] Create a new Default VPC:
  - [ ] Refresh console, go to **Actions** → **Create default VPC**.
  - [ ] Click **Create default VPC** button.

### Task 2: Launch an EC2 Instance
- [ ] Ensure you are in the **US East (N. Virginia) us-east-1** Region.
- [ ] Navigate to **EC2**:
  - [ ] Click on the **Services** menu → EC2 in the Compute section.
- [ ] Launch a new instance:
  - [ ] Click **Instances** → **Launch Instances**.
  - [ ] Name: Enter **"MyEC2Server"**.
  - [ ] Search and select **Amazon Linux 2 AMI**.
  - [ ] For Instance Type: Select **t2.micro**.
- [ ] Configure the Key Pair:
  - [ ] Click **Create a new key pair**.
  - [ ] Name: **SecKey** with type **RSA** and format **.pem**.
- [ ] Modify Network Settings:
  - [ ] Enable **Auto-assign public IP**.
  - [ ] Create a security group: **MyEC2Server_SG**.
    - [ ] Description: **Security Group to allow traffic to EC2**.
    - [ ] Add **Security Group Rules**:
      - [ ] SSH (already present).
      - [ ] HTTP: **Type: HTTP**, **Source: Anywhere**.
- [ ] Proceed to launch the instance with default settings.
  - [ ] Click **Launch Instance**.
- [ ] View Instance:
  - [ ] Choose **View all Instances**.
  - [ ] Wait for instance state to become **Running** and health check status to pass 2/2.

### Task 3: SSH into EC2 Instance
- [ ] Select the **MyEC2Server** instance and click **Connect**.
- [ ] Use **EC2 Instance Connect** and click **Connect**.
- [ ] A new tab opens where you can execute Linux commands.

### Task 4: Install an Apache Server
  ```bash
  # Switch to root user
  sudo su

  # Update system packages
  yum -y update

  # Install Apache Web Server
  yum install httpd -y

  # Start and Enable the Web Server
  systemctl start httpd
  systemctl enable httpd

  # Verify Web Server Status
  systemctl status httpd
  ```

- [ ] Test Web Server:
  - [ ] Enter the **Public IPv4 address** of your instance in a web browser.

### Task 6: Create a Web Page
- [ ] Add content to the web page:
  ```bash
  echo "<html>Hi Ifeanyi, I am a public page</html>" > /var/www/html/index.html
  ```
- [ ] Restart the Web Server:
  ```bash
  systemctl restart httpd
  ```
- [ ] Access your content in a web browser with:
  - [ ] **http://<Your_Public_IPv4_Address>/index.html**

</details>

<details> 
  <summary>Project 9 - Configure Load Balancer and Auto Scaling Group with Launch templates</summary>
  
  ###
     
  <a href="" target="_blank"><img src="https://github.com/user-attachments/assets/055f47bd-07b2-4129-b479-fbd5f7a64eeb" width="720" height="400" /></a>
  
  ###
  
  <img src="https://github.com/user-attachments/assets/59e9595b-b4e8-45e8-a8d3-d0e4b3d36adc" width="720" height="520" />

## ✅ Task 1: Create a Security Group for Load Balancer
- [ ] Set **default AWS Region** to **US East (N. Virginia) us-east-1**.
- [ ] Navigate to **EC2** > **Security Groups**.
- [ ] Click **Create security group**.
- [ ] **Security group name:** `Load-balancer-SG`
- [ ] **Description:** `Security group for Load balancer`
- [ ] **VPC:** Select **Default VPC**
- [ ] **Add Inbound Rule:**
  - Type: `HTTP`
  - Source: `Custom`
  - Value: `0.0.0.0/0`
- [ ] Click **Create security group**.

## ✅ Task 2: Create a Security Group for Launch Template
- [ ] Click **Create security group**.
- [ ] **Security group name:** `Launch-template-SG`
- [ ] **Description:** `Security group for Launch template`
- [ ] **VPC:** Select **Default VPC**
- [ ] **Add Inbound Rules:**
  - Type: `SSH`
  - Source: `Custom`
  - Value: `0.0.0.0/0`
  - Type: `HTTP`
  - Source: `Custom`
  - Value: `Load-balancer-SG`
- [ ] Click **Create security group**.

## ✅ Task 3: Create a Key Pair for Launch Template
- [ ] Navigate to **EC2** > **Key Pairs**.
- [ ] Click **Create key pair**.
- [ ] **Name:** `MyKeyPair`
- [ ] **File format:** `pem` (Linux & Mac) or `ppk` (Windows)
- [ ] Click **Create key pair**.

## ✅ Task 4: Create a Launch Template
- [ ] Navigate to **EC2** > **Launch Templates**.
- [ ] Click **Create launch template**.
- [ ] **Launch template name:** `MylabsLC`
- [ ] **Template version description:** `Launch template for Mydemo`
- [ ] Select **Amazon Linux 2 AMI (HVM), SSD Volume Type**
- [ ] **Instance type:** `t2.micro`
- [ ] **Key pair:** `MyKeyPair`
- [ ] **Subnet:** Choose any subnet
- [ ] **Security groups:** `Launch-template-SG`
- [ ] Expand **Advanced details** > **User data:**
  ```bash
  #!/bin/bash
  sudo su
  yum update -y
  yum install -y httpd
  systemctl start httpd
  systemctl enable httpd
  echo "Hello World from $(hostname -f)" > /var/www/html/index.html
  echo "Healthy" > /var/www/html/health.html
  ```
- [ ] Click **Create launch template**.

## ✅ Task 5: Create Target Group
- [ ] Navigate to **EC2** > **Target Groups**.
- [ ] Click **Create Target Group**.
- [ ] **Target Type:** `Instances`
- [ ] **Name:** `web-server-TG`
- [ ] **Protocol:** `HTTP`
- [ ] **Port:** `80`
- [ ] **Health check protocol:** `HTTP`
- [ ] **Path:** `/health.html`
- [ ] Click **Next** > **Create target group**.

## ✅ Task 6: Create Load Balancer
- [ ] Navigate to **EC2** > **Load Balancers**.
- [ ] Click **Create load balancer**.
- [ ] Choose **Application Load Balancer**.
- [ ] **Name:** `Web-server-LB`
- [ ] **Scheme:** `Internet-facing`
- [ ] **IP address type:** `IPv4`
- [ ] **VPC:** `Default`
- [ ] **Availability Zones:** `us-east-1a` and `us-east-1b`
- [ ] **Security Group:** `Load-balancer-SG`
- [ ] **Listener:** Select **Target group** created earlier.
- [ ] Click **Create Load Balancer**.

## ✅ Task 7: Create an Auto Scaling Group
- [ ] Navigate to **EC2** > **Auto Scaling Groups**.
- [ ] Click **Create Auto Scaling group**.
- [ ] **Name:** `My-ASG`
- [ ] **Launch template:** `MylabsLC`
- [ ] **VPC:** `Default`
- [ ] **Subnets:** `us-east-1a`, `us-east-1b`
- [ ] **Attach to Load Balancer:** `web-server-TG`
- [ ] **Health Check Type:** `EC2 + ELB`
- [ ] **Health Check Grace Period:** `60 seconds`
- [ ] **Desired Capacity:** `2`
- [ ] **Minimum Capacity:** `1`
- [ ] **Maximum Capacity:** `4`
- [ ] **Scaling Policy:** `Target tracking` > `CPU Utilization` > `30%`
- [ ] Click **Create Auto Scaling Group**.

## ✅ Task 8: SSH into EC2 Instance
- [ ] Use SSH to connect to the EC2 instance.
- [ ] Syntax : ssh -i keypair_filename UserName@publicIPAddress (enter the username and public IP address)
- [ ] Example : ssh -i ec2_connect.pem ec2-user@54.172.93.175  --> Click Enter

## ✅ Task 9: Test Auto Scaling and Load Balancer
- [ ] Copy **Load Balancer DNS**.
- [ ] Paste in browser to confirm traffic routing.
- [ ] Stop one of the EC2 instance.
- [ ] Check browser for change in server.

## ✅ Task 10: Delete AWS Resources
### (I) Delete Auto Scaling Group
- [ ] Navigate to **EC2** > **Auto Scaling Groups**.
- [ ] Select `My-ASG` > **Actions** > **Delete**.
- [ ] Confirm by typing `delete`.

### (II) Delete Launch Template
- [ ] Navigate to **EC2** > **Launch Templates**.
- [ ] Select `MylabsLC` > **Actions** > **Delete template**.

### (III) Delete Load Balancer
- [ ] Navigate to **EC2** > **Load Balancers**.
- [ ] Select `Web-server-LB` > **Actions** > **Delete**.

### (IV) Delete Target Group
- [ ] Navigate to **EC2** > **Target Groups**.
- [ ] Select `web-server-TG` > **Actions** > **Delete**.
- [ ] Sign out of AWS.

---
🎉 **Congratulations! You have successfully completed the AWS Auto Scaling and Load Balancer Lab!**

</details>



