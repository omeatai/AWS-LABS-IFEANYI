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
     
  <a href="https://youtu.be/hiFPfd2WG8A" target="_blank"><img src="https://github.com/user-attachments/assets/055f47bd-07b2-4129-b479-fbd5f7a64eeb" width="720" height="400" /></a>
  
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

<details> 
  <summary>Project 10 - Automating S3 File Copy and Transfer with AWS Lambda </summary>
  
  ###
     
  <a href="https://youtu.be/hiFPfd2WG8A" target="_blank"><img src="https://github.com/user-attachments/assets/ef94c27f-0d15-48db-b028-200eb2923e56" width="720" height="400" /></a>
  
  ###
  
  <img src="https://github.com/user-attachments/assets/93ee9208-4e31-4faf-b506-a0bb3f85c85d" width="720" height="520" />

## ✅ Task 1: Create Two Amazon S3 Buckets

### Create Source Bucket

- [ ] # Set the default **AWS Region** to **US East (N. Virginia) (us-east-1)**.
- [ ] # Navigate to **Services > S3** under the **Storage** section.
- [ ] # Click on **Create Bucket**.
- [ ] # Enter **Bucket Name**: `mysourcebucket12345` _(Choose a unique name)_.
- [ ] # Select **AWS Region**: **US East (N. Virginia) (us-east-1)**.
- [ ] # Leave other settings as **default** and click **Create bucket**.
- [ ] # Select your bucket and **copy the ARN**.
- [ ] # Save the **source bucket ARN** in a text file: arn:aws:s3:::mysourcebucket12345

### Create Destination Bucket

- [ ] # Click on **Create Bucket** again.
- [ ] # Enter **Bucket Name**: `mydestinationbucket12345` _(Choose a unique name)_.
- [ ] # Select **AWS Region**: **US East (N. Virginia) (us-east-1)**.
- [ ] # Leave other settings as **default** and click **Create bucket**.
- [ ] # Select your bucket and **copy the ARN**.
- [ ] # Save the **destination bucket ARN** in a text file: arn:aws:s3:::mydestinationbucket12345

## ✅ Task 2: Create a Lambda Function

- [ ] # Ensure you are in the **US East (N. Virginia) (us-east-1)** region.
- [ ] # Navigate to **Services > Lambda** under the **Compute** section.
- [ ] # Click on **Create Function**.
- [ ] # Select **Author from scratch**.
- [ ] # Enter **Function Name**: `mylambdafunction`.
- [ ] # Choose **Runtime**: `Python 3.13`.
- [ ] # Under **Permissions**, select **Change default execution role**.
- [ ] # Choose **Use an existing role** and select `Lambda_role`.
- [ ] # Click **Create function**.

## ✅ Task 3: Add Code to Lambda Function

- [ ] # Scroll down to the **Code source** section.
- [ ] # Remove existing code in `lambda_function.py`.
- [ ] # Copy and paste the following **Python** code into `lambda_function.py`:

```python
import boto3
import urllib.parse

def lambda_handler(event, context):
    s3 = boto3.client('s3')

    source_bucket = "mysourcebucket12345"
    destination_bucket = "mydestinationbucket12345"

    # Extract the object key from the event
    object_key = event['Records'][0]['s3']['object']['key']

    # URL encode the source object key
    copy_source = urllib.parse.quote(f"{source_bucket}/{object_key}")

    # Set up the parameters for the copy operation
    copy_params = {
        'Bucket': destination_bucket,
        'CopySource': copy_source,
        'Key': object_key
    }

    try:
        # Perform the copy operation
        result = s3.copy_object(**copy_params)
        print("S3 object copy successful.")
    except Exception as e:
        print(f"Error copying object: {str(e)}")
```

- [ ] # Replace mysourcebucket12345 and mydestinationbucket12345 with your actual bucket names.
- [ ] # Click Deploy to save the function.

## ✅ Task 4: Adding Triggers to Lambda Function

- [ ] # Scroll up to Function overview and click + Add trigger.
- [ ] # Select S3 from the trigger list.
- [ ] # Set Bucket: mysourcebucket12345.
- [ ] # Choose Event Type: All object create events.
- [ ] # Enable Recursive invocation to prevent failures when uploading multiple files.
- [ ] # Check the acknowledge option.
- [ ] # Click Add.

## ✅ Task 5: Test Lambda Function

### Upload a Test Image

- [ ] # Download a test image and save it as image.jpeg (Do not rename it to variations like image (2).jpeg).
- [ ] # Go to S3 Bucket list and open the source bucket (mysourcebucket12345).
- [ ] # Click Upload > Add files.
- [ ] # Select image.jpeg and click Upload.

### Verify the File Transfer

- [ ] # Open the destination bucket (mydestinationbucket12345).
- [ ] # Ensure that a copy of image.jpeg is present in the destination bucket.

## ✅ Task 6: (Optional) Debugging Lambda Function Using CloudWatch

- [ ] # If the file is not copied, debug the Lambda function using CloudWatch.
- [ ] # Navigate to Services > CloudWatch.
- [ ] # Select Logs > Log Groups.
- [ ] # Find the log group /aws/lambda/mylambdafunction.
- [ ] # Select the latest log stream.
- [ ] # Expand Log events to check for error messages.
- [ ] # If sourceBucket is not defined, update the Lambda function with the correct bucket names.
- [ ] # Click Deploy after making corrections.

---
🎉 **Congratulations! You have successfully automated S3 file transfers using AWS Lambda. 🚀**

</details>

<details> 
  <summary>Project 11 - Managing IAM Users and Groups in AWS </summary>
  
  ###
     
  <a href="https://youtu.be/gFaFEb3K9EI" target="_blank"><img src="https://github.com/user-attachments/assets/69448d93-e021-4c3e-97b8-97e1de828596" width="720" height="400" /></a>

  ###
  
  <img src="https://github.com/user-attachments/assets/f2b269aa-72be-4695-a678-e84cbce0bbb9" width="720" height="520" />

## ✅ Task 1: Create IAM Users

- [ ] # Set the default **AWS Region** to **US East (N. Virginia) (us-east-1)**.
- [ ] # Navigate to **Services > IAM** under **Security, Identity, & Compliance**.
- [ ] # In the IAM dashboard, select **Users** from the left panel.
- [ ] # Click **Create User**.
- [ ] # Under **User Details**, fill in the following:
  - **User name**: `John` (or any desired name).
  - **Check** the **Provide user access to the AWS Management Console - optional** checkbox.
  - **Select** `Custom password` under **Console Password**.
  - **Enter Password**: `mylabs@123` (or any desired password).
  - **Uncheck** `Users must create a new password at the next sign-in (recommended)`.
  - Click **Next**.
- [ ] # In the **Set permissions** section, keep settings as default and click **Next**.
- [ ] # Under **Tags**, click **Add new tag**:
  - **Key**: `Dev-Team`
  - **Value**: `Developers`
- [ ] # Click **Create User**.
- [ ] # If you see an error, ignore it and click **Close**.
- [ ] # Click **Return to users list** and then **Continue**.
- [ ] # Repeat the same steps to create an IAM user named **Sarah** with the same **Dev-Team** tag.
- [ ] # Repeat the steps to create IAM users named **Ted** and **Rita** with the following details:
  - **Custom password**: `mylabs@123`
  - **Key**: `HR-Team`
  - **Value**: `HR`
- [ ] # You have now created **four IAM users**: `John, Sarah, Ted, and Rita`.

## ✅ Task 2: Create IAM Groups and Add IAM Users

### Create **Dev-Team** Group and Add Users
- [ ] # Navigate to **User groups** in the left panel.
- [ ] # Click **Create group**.
- [ ] # **User group name**: `Dev-Team`
- [ ] # Scroll down and **add users**: `John` and `Sarah`.
- [ ] # Under **Attach permissions policies**, search for:
  - `AmazonEC2ReadOnlyAccess`
  - `AmazonS3ReadOnlyAccess`
- [ ] # **Select both policies** (These provide read access for EC2 and S3).
- [ ] # **Review** all details and click **Create group**.

### Create **HR-Team** Group and Add Users
- [ ] # Click **Create group**.
- [ ] # **User group name**: `HR-Team`
- [ ] # Scroll down and **add users**: `Ted` and `Rita`.
- [ ] # Under **Attach permissions policies**, search for:
  - `Billing`
- [ ] # **Select the Billing policy** (grants billing-related permissions).
- [ ] # **Review** all details and click **Create group**.

✅ # Congratulations! You have successfully created IAM users, groups, and assigned permissions in AWS. 🚀

</details> 
  
<details> 
  <summary>Project 12 - Configuring a Custom VPC with Public and Private Subnets </summary>
  
  ###
     
  <a href="https://youtu.be/9jk2d_99Axg" target="_blank"><img src="https://github.com/user-attachments/assets/a6de47ec-2c0d-467f-a0ca-178b97d215e0" width="720" height="400" /></a>

  ###
  
  <img src="https://github.com/user-attachments/assets/42f30705-4bfc-4ce2-aaf1-faf37755903a" width="920" height="520" />

# Project: Configuring a Custom VPC with Public and Private Subnets in AWS ✅

## ✅ Task 1: Create a New VPC

- [ ] # Once signed in, set the **AWS Region** to **US East (N. Virginia) (us-east-1)**.
- [ ] # Ensure you are in the **US East (N. Virginia) (us-east-1)** region.
- [ ] # Navigate to **VPC** by:
  - Clicking on **Services** (top menu).
  - Searching for **VPC** and selecting it under **Networking & Content Delivery**.
- [ ] # Click on **Your VPCs** (left menu).
- [ ] # Click on **Create VPC**.
- [ ] # In the **Create VPC** form:
  - Select **VPC Only**.
  - **Name tag**: Enter `MyVPC`.
  - **IPv4 CIDR block**: Enter `10.0.0.0/16`.
  - **IPv6 CIDR block**: Ensure **No IPv6 CIDR Block** is selected.
  - **Tenancy**: Keep as **Default**.
- [ ] # Click on **Create VPC**.
- [ ] # Confirm that the VPC appears in the list.

---

## ✅ Task 2: Create Public and Private Subnets

### **Create a Public Subnet**
- [ ] # Click on **Subnets** (left menu).
- [ ] # Click on **Create subnet**.
- [ ] # In the **Create Subnet** form:
  - **VPC ID**: Select `MyVPC`.
  - **Subnet Name**: Enter `MyPublicSubnet`.
  - **Availability Zone**: Select `us-east-1a`.
  - **IPv4 CIDR block**: Enter `10.0.1.0/24`.
- [ ] # Click **Create subnet**.

### **Create a Private Subnet**
- [ ] # Click on **Create subnet** again.
- [ ] # In the **Create Subnet** form:
  - **VPC ID**: Select `MyVPC`.
  - **Subnet Name**: Enter `MyPrivateSubnet`.
  - **Availability Zone**: Select `us-east-1b`.
  - **IPv4 CIDR block**: Enter `10.0.2.0/24`.
- [ ] # Click **Create subnet**.

---

## ✅ Task 3: Create and Attach an Internet Gateway

- [ ] # Click on **Internet Gateways** (left menu).
- [ ] # Click **Create internet gateway**.
- [ ] # **Name Tag**: Enter `MyInternetGateway`.
- [ ] # Click **Create internet gateway**.
- [ ] # Select the created Internet Gateway from the list.
- [ ] # Click on **Actions > Attach to VPC**.
- [ ] # Select **MyVPC** from the dropdown list.
- [ ] # Click **Attach internet gateway**.

---

## ✅ Task 4: Create and Configure Route Tables

### **Create a Public Route Table**
- [ ] # Click on **Route Tables** (left menu).
- [ ] # Click on **Create route table**.
- [ ] # **Name**: Enter `PublicRouteTable`.
- [ ] # **VPC**: Select `MyVPC`.
- [ ] # Click **Create route table**.

### **Create a Private Route Table**
- [ ] # Click on **Create route table** again.
- [ ] # **Name**: Enter `PrivateRouteTable`.
- [ ] # **VPC**: Select `MyVPC`.
- [ ] # Click **Create route table**.

### **Associate Public Subnet with the Public Route Table**
- [ ] # Select `PublicRouteTable` from the list.
- [ ] # Go to **Subnet Associations** tab.
- [ ] # Click **Edit subnet associations**.
- [ ] # Select **MyPublicSubnet** from the list.
- [ ] # Click **Save associations**.

### **Associate Private Subnet with the Private Route Table**
- [ ] # Select `PrivateRouteTable` from the list.
- [ ] # Go to **Subnet Associations** tab.
- [ ] # Click **Edit subnet associations**.
- [ ] # Select **MyPrivateSubnet** from the list.
- [ ] # Click **Save associations**.

### **Configure Public Route Table to Allow Internet Traffic**
- [ ] # Select `PublicRouteTable` from the list.
- [ ] # Go to **Routes** tab.
- [ ] # Click **Edit routes**.
- [ ] # Click **Add route**.
- [ ] # Set:
  - **Destination**: `0.0.0.0/0`
  - **Target**: Select **Internet Gateway** (`MyInternetGateway`).
- [ ] # Click **Save changes**.

✅ **Congratulations! You have successfully configured a custom VPC with public and private subnets in AWS. 🚀**

</details> 

<details> 
  <summary>Project 13 - Configuring NAT Gateways with AWS Subnets </summary>
  
  ###
     
  <a href="https://youtu.be/E8-pe2m5qYE" target="_blank"><img src="https://github.com/user-attachments/assets/e5e81af1-cc92-4cd9-8f33-0b30f8b88418" width="720" height="400" /></a>

  ###
  
  <img src="https://github.com/user-attachments/assets/321db31a-370c-4809-82d0-832da55e9e60" width="920" height="520" />

# Project 13: Deploying a Secure AWS NAT Network with Public and Private Subnets ✅

## **Task 1: Create a VPC**
- [ ] Ensure the default AWS Region is **US East (N. Virginia) (us-east-1)**.
- [ ] Navigate to **VPC > Your VPCs**.
- [ ] Click **Create VPC**.
- [ ] Select **VPC Only**.
- [ ] Set **Name Tag**: `MyVPC`.
- [ ] Set **IPv4 CIDR Block**: `10.0.0.0/16`.
- [ ] Ensure **No IPv6 CIDR Block** is selected.
- [ ] Ensure **Tenancy** is set to **Default**.
- [ ] Click **Create VPC**.

## **Task 2: Create Public and Private Subnets**
- [ ] Navigate to **VPC > Subnets**.
- [ ] Click **Create Subnet**.

### **Create Public Subnet**
- [ ] Select **VPC ID**: `MyVPC`.
- [ ] Set **Subnet Name**: `MyPublicSubnet`.
- [ ] Select **Availability Zone**: `No Preference`.
- [ ] Set **IPv4 CIDR Block**: `10.0.0.0/24`.
- [ ] Click **Create Subnet**.
- [ ] Select `MyPublicSubnet`, go to **Actions > Edit subnet settings**.
- [ ] Enable **Auto-assign public IPv4 address**.
- [ ] Click **Save**.

### **Create Private Subnet**
- [ ] Click **Create Subnet**.
- [ ] Select **VPC ID**: `MyVPC`.
- [ ] Set **Subnet Name**: `MyPrivateSubnet`.
- [ ] Select **Availability Zone**: `No Preference`.
- [ ] Set **IPv4 CIDR Block**: `10.0.1.0/24`.
- [ ] Click **Create Subnet**.

## **Task 3: Create and Attach an Internet Gateway**
- [ ] Navigate to **VPC > Internet Gateways**.
- [ ] Click **Create Internet Gateway**.
- [ ] Set **Name Tag**: `MyIGW`.
- [ ] Click **Create Internet Gateway**.
- [ ] Select `MyIGW`, go to **Actions > Attach to VPC**.
- [ ] Select `MyVPC`.
- [ ] Click **Attach Internet Gateway**.

## **Task 4: Create and Configure a Public Route Table**
- [ ] Navigate to **VPC > Route Tables**.
- [ ] Click **Create Route Table**.
- [ ] Set **Name Tag**: `PublicRouteTable`.
- [ ] Select **VPC**: `MyVPC`.
- [ ] Click **Create Route Table**.
- [ ] Select `PublicRouteTable`, go to **Routes tab > Edit Routes**.
- [ ] Click **Add Route**.
- [ ] Set **Destination**: `0.0.0.0/0`.
- [ ] Set **Target**: `MyIGW (Internet Gateway)`.
- [ ] Click **Save Changes**.
- [ ] Select `PublicRouteTable`, go to **Subnet Associations > Edit Subnet Associations**.
- [ ] Select **MyPublicSubnet**.
- [ ] Click **Save Associations**.

## **Task 5: Launch an EC2 Instance in Public Subnet**
- [ ] Navigate to **EC2 > Instances**.
- [ ] Click **Launch Instances**.
- [ ] Set **Name**: `MyPublicServer`.
- [ ] Select **Amazon Linux 2 AMI**.
- [ ] Choose **Instance Type**: `t2.micro`.
- [ ] Under **Key Pair**, click **Create new Key Pair**.
  - **Key Pair Name**: `MyKey`.
  - **Key Pair Type**: `RSA`.
  - **Private Key Format**: `.pem`.
- [ ] Click **Create Key Pair**.
- [ ] Under **Network Settings**, click **Edit**.
  - **VPC**: `MyVPC`.
  - **Subnet**: `MyPublicSubnet`.
  - **Auto-assign Public IP**: **Enabled**.
  - **Create new Security Group**:
    - **Name**: `MyEC2Server_SG`
    - **Description**: `Security Group to allow traffic to EC2`
    - **Inbound Rule**: **Allow SSH (Port 22) from Anywhere**.
- [ ] Click **Launch Instance**.
- [ ] Click **View all Instances** and wait for status **Running**.

## **Task 6: Launch an EC2 Instance in Private Subnet**
- [ ] Click **Launch Instances**.
- [ ] Set **Name**: `MyPrivateServer`.
- [ ] Select **Amazon Linux 2 AMI**.
- [ ] Choose **Instance Type**: `t2.micro`.
- [ ] Under **Key Pair**, select **MyKey**.
- [ ] Under **Network Settings**, click **Edit**.
  - **VPC**: `MyVPC`.
  - **Subnet**: `MyPrivateSubnet`.
  - **Auto-assign Public IP**: **Disabled**.
  - **Select Existing Security Group**: `MyEC2Server_SG`.
- [ ] Click **Launch Instance**.
- [ ] Click **View all Instances** and wait for status **Running**.
- [ ] Note the **Private IP Address** of `MyPrivateServer`.

## **Task 7: SSH into Public and Private EC2 Instances**

### **SSH into MyPublicServer**
- [ ] Select `MyPublicServer`, click **Connect**.
- [ ] Choose **EC2 Instance Connect**, click **Connect**.
- [ ] Switch to root user:  
  ```bash
  sudo su
  ```
- [ ]  Update instance:
  ```bash
  yum -y update
  ```
  
### **SSH into MyPublicServer**
- [ ] Open MyKey.pem in a text editor on your local machine and copy its contents.
- [ ] In MyPublicServer, create the key file:
  ```bash
  vi MyKey.pem
  ```
- [ ] Press i to insert, paste the key, then press Esc and type :wq to save.
- [ ] Set correct permissions:
  ```bash
  chmod 400 MyKey.pem
  ```
- [ ] SSH into MyPrivateServer:
  ```bash
  ssh ec2-user@<Private IP> -i MyKey.pem
  ```
- [ ] Switch to root user:
  ```bash
   sudo su
  ```
- [ ] Attempt update:
  ```bash
  yum -y update
  ```
- [ ] Expected result: No internet access.

## **Task 8: Create a NAT Gateway**
 - [ ] Navigate to VPC > NAT Gateways.
 - [ ] Click Create NAT Gateway.
 - [ ] Set Name Tag: MyNATGateway.
 - [ ] Select Subnet: MyPublicSubnet.
 - [ ] Click Allocate Elastic IP.
 - [ ] Click Create NAT Gateway.
 - [ ] Wait for status Available.

## **Task 9: Update Private Route Table for NAT Gateway**
 - [ ] Navigate to VPC > Route Tables.
 - [ ] Select Main Route Table.
 - [ ] Click Edit Routes.
 - [ ] Click Add Route.
 - [ ] Set Destination: 0.0.0.0/0.
 - [ ] Set Target: MyNATGateway.
 - [ ] Click Save Changes.

## **Task 10: Test Internet Connection from Private Subnet**
- [ ] SSH into MyPublicServer.
- [ ]  Switch to root:
```bash
   sudo su
```
- [ ] SSH into MyPrivateServer: 
```bash
   ssh ec2-user@<Private IP> -i MyKey.pem
```
- [ ] Switch to root:
```bash
   sudo su
```
- [ ] Run updates: 
```bash
   yum -y update
```
- [ ] Expected result: Update should complete successfully, confirming internet access via NAT Gateway.

Completion:
✅ AWS VPC with Public & Private Subnets Successfully Deployed!

</details> 

<details> 
  <summary>Project 14 - Deploying a Secured Multi-Layered VPC on AWS </summary>
  
  ###
     
  <a href="" target="_blank"><img src="https://github.com/user-attachments/assets/0b86b6e0-69fe-4306-973d-d63478f2eb22" width="720" height="400" /></a>

  ###
  
  <img src="https://github.com/user-attachments/assets/29fee6cf-a194-4ea3-be7e-be2071fee8f7" width="920" height="520" />

# Project 14: Deploying a Secured Multi-Layered VPC on AWS ✅

## **Task 1: Create a New VPC**
- [ ] Set AWS **Region** to **US East (N. Virginia) (us-east-1)**.
- [ ] Navigate to **VPC > Your VPCs**.
- [ ] Click **Create VPC**.
- [ ] Select **VPC Only**.
- [ ] Name: `my_VPC`.
- [ ] **IPv4 CIDR Block**: `10.0.0.0/16`.
- [ ] **IPv6 CIDR Block**: `No IPv6 CIDR Block`.
- [ ] **Tenancy**: `Default`.
- [ ] Click **Create VPC**.

## **Task 2: Create and Attach an Internet Gateway**
- [ ] Navigate to **VPC > Internet Gateways**.
- [ ] Click **Create Internet Gateway**.
- [ ] Name: `my_IGW`.
- [ ] Click **Create Internet Gateway**.
- [ ] Select `my_IGW` from the list.
- [ ] Click **Actions > Attach to VPC**.
- [ ] Select `my_VPC`.
- [ ] Click **Attach Internet Gateway**.

## **Task 3: Create Two Subnets**
- [ ] Navigate to **VPC > Subnets**.
- [ ] Click **Create Subnet**.

### **Create Public Subnet**
- [ ] **VPC ID**: `my_VPC`.
- [ ] **Name**: `public_subnet`.
- [ ] **Availability Zone**: `No Preference`.
- [ ] **IPv4 CIDR Block**: `10.0.1.0/24`.
- [ ] Click **Create Subnet**.

### **Create Private Subnet**
- [ ] Click **Create Subnet**.
- [ ] **VPC ID**: `my_VPC`.
- [ ] **Name**: `private_subnet`.
- [ ] **Availability Zone**: `No Preference`.
- [ ] **IPv4 CIDR Block**: `10.0.2.0/24`.
- [ ] Click **Create Subnet**.

## **Task 4: Create Route Tables and Configure Routes**
- [ ] Navigate to **VPC > Route Tables**.
- [ ] Click **Create Route Table**.

### **Create Public Route Table**
- [ ] Name: `public_route`.
- [ ] **VPC**: `my_VPC`.
- [ ] Click **Create Route Table**.

### **Create Private Route Table**
- [ ] Click **Create Route Table**.
- [ ] Name: `private_route`.
- [ ] **VPC**: `my_VPC`.
- [ ] Click **Create Route Table**.

### **Configure Public Route**
- [ ] Select `public_route`.
- [ ] Go to **Routes > Edit Routes**.
- [ ] Click **Add Route**.
- [ ] **Destination**: `0.0.0.0/0`.
- [ ] **Target**: `my_IGW (Internet Gateway)`.
- [ ] Click **Save Changes**.

### **Associate Public Subnet**
- [ ] Select `public_route`.
- [ ] Click **Edit Subnet Associations**.
- [ ] Select `public_subnet`.
- [ ] Click **Save Associations**.

### **Associate Private Subnet**
- [ ] Select `private_route`.
- [ ] Click **Edit Subnet Associations**.
- [ ] Select `private_subnet`.
- [ ] Click **Save Associations**.

## **Task 5: Create a Security Group**
- [ ] Navigate to **VPC > Security Groups**.
- [ ] Click **Create Security Group**.
- [ ] Name: `my_securitygroup`.
- [ ] Description: `Security group for multilayered VPC`.
- [ ] **VPC**: `my_VPC`.

### **Inbound Rules**
- [ ] **SSH**:
  - **Type**: SSH.
  - **Source**: `0.0.0.0/0`.
- [ ] **All ICMP - IPv4**:
  - **Type**: All ICMP - IPv4.
  - **Source**: Anywhere IPv4.

- [ ] Click **Create Security Group**.

## **Task 6: Create and Configure Network ACL**
- [ ] Navigate to **VPC > Network ACLs**.
- [ ] Click **Create Network ACL**.
- [ ] Name: `my_NACL`.
- [ ] **VPC**: `my_VPC`.
- [ ] Click **Create Network ACL**.

### **Inbound Rules**
- [ ] **SSH** (Rule 100):  
  - **Type**: SSH (22).  
  - **Source**: `0.0.0.0/0`.  
  - **Allow/Deny**: Allow.  
- [ ] **All ICMP - IPv4** (Rule 200):  
  - **Type**: All ICMP - IPv4.  
  - **Source**: `0.0.0.0/0`.  
  - **Allow/Deny**: Allow.

- [ ] Click **Save Changes**.

### **Outbound Rules**
- [ ] **All ICMP - IPv4** (Rule 100):  
  - **Type**: All ICMP - IPv4.  
  - **Destination**: `0.0.0.0/0`.  
  - **Allow/Deny**: Allow.
- [ ] **Custom TCP Rule** (Rule 200):  
  - **Type**: Custom TCP Rule.  
  - **Port Range**: `1024 - 65535`.  
  - **Destination**: `0.0.0.0/0`.  
  - **Allow/Deny**: Allow.

- [ ] Click **Save Changes**.

### **Associate NACL with Subnets**
- [ ] Select `my_NACL`.
- [ ] Go to **Subnet Associations**.
- [ ] Click **Edit Subnet Associations**.
- [ ] Select **public_subnet** and **private_subnet**.
- [ ] Click **Save Changes**.

## **Task 7: Launch Two EC2 Instances**
- [ ] Navigate to **EC2 > Instances**.
- [ ] Click **Launch Instances**.

### **Public Instance**
- [ ] Name: `public_instance`.
- [ ] **AMI**: `Amazon Linux 2 AMI`.
- [ ] **Instance Type**: `t2.micro`.
- [ ] **Key Pair**: Create `WhizKey.pem`.
- [ ] **Network Settings**:
  - **VPC**: `my_VPC`.
  - **Subnet**: `public_subnet`.
  - **Auto-assign Public IP**: Enabled.
  - **Security Group**: `my_securitygroup`.
- [ ] Click **Launch Instance**.

### **Private Instance**
- [ ] Name: `private_instance`.
- [ ] **Key Pair**: Use `WhizKey.pem`.
- [ ] **VPC**: `my_VPC`.
- [ ] **Subnet**: `private_subnet`.
- [ ] **Auto-assign Public IP**: Disabled.
- [ ] **Security Group**: `my_securitygroup`.
- [ ] Click **Launch Instance**.

## **Task 8: Test Connectivity**
- [ ] Copy **Public IPv4 Address** of `public_instance`.
- [ ] Select EC2 Instance Connect option and click on Connect button.
- [ ] A new tab will open in the browser where you can execute the CLI Commands.
- [ ] For MAC & Linux Users:
  - Open Terminal application in your local system.
  - Navigate to the location where .pem key is downloaded and stored in your local.
  - To update Permissions, run command
    -  Syntax : chmod 400 keypair_filename
    -  Example : chmod 400 ec2_connect.pem
  - User Name of the server:
    -  Amazon Linux AMI : ec2-user
    -  Ubuntu AMI : ubuntu
    -  OPENVPN AMI : root
  - To SSH and connect to the EC2 Instance, Enter the following command:
    -  Syntax : ssh -i keypair_filename UserName@publicIPAddress (enter the username and public IP address)
    -  Example : ssh -i ec2_connect.pem ec2-user@54.172.93.175  --> Click Enter
    -  Up next, type yes and Enter, you will be successfully logged into EC2 Instance.
- [ ] For Windows (10,11) Users in command prompt and PowerShell:
    -  Use PEM file from the EC2 Instance.
    -  Once instance is launched, click on connect button and go to SSH client section.
    -  Copy the SSH client key.
    -  Open command prompt or PowerShell in your windows.
    -  Check where the PEM file has downloaded in your local.
    -  Change your path to downloads section. Example of command <cd downloads>
    -  With the key which you have copied, we have to use now: 
      ```bs
      ssh -i "<your pem file name>" ec2-user@ec2-<your ip address>.compute-1.amazonaws.com
      ```
    - You have successfully connected to ec2 instance via windows PowerShell.
- [ ] For Microsoft Windows Users( Putty):
    - Download putty and puttygen from this link : https://www.chiark.greenend.org.uk/~sgtatham/putty/releases/0.74.html
    - To convert your key pair .pem to .ppk.
      - Open PuttyGen.
      - Click on Load
      - Click on All files to show your .pem file and select the .pem keypair file.
      - And Click on open, You will get uccess message if done correctly.
      - Click on the Save Private Key button.
      - Enter keypairname and Save.
      - keypairname.ppk file will be saved to your local machine.
    - Navigate to the EC2 instance page and get the public IP of the machine.
    - Open Putty
      - Host Name: Enter the public IP address.
      - Click SSH, select AUTH, and again click credentials, then Browse to select the private key (.ppk) that you converted from the .pem file.
      - Click on Open
      - Select accept to connect to the machine
      - If you are using Amazon Linux AMI  for the lab:
        - Enter user name: ec2-user and hit Enter.
      - If you are using Ubuntu AMI for the lab:
        - Enter user name: ubuntu and hit Enter.
      - If you are using OPENVPN AMI for the lab:
        - Enter user name: root and hit Enter.
      - You will see the console after a successful login.         
- [ ] Copy **Private IPv4 Address** of `private_instance`.
- [ ] SSH into `public_instance`:
  ```bash
  ssh -i WhizKey.pem ec2-user@<Public_IP>
  ```
- [ ] Ping private_instance from public_instance:
  ```bash
  ping <Private_IP>
  ```
- [ ] Confirm a successful response.

✅ Multi-Layered VPC Successfully Deployed!

</details> 
