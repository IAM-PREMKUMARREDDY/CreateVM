# CreateVM
Certainly! Here's a **step-by-step procedure** to create a **Resource Group** and a **Windows Virtual Machine (VM)** on your **Azure Free Trial** subscription. 

### **Step 1: Create a Resource Group**

1. **Log in to the Azure Portal**  
   Go to the [Azure Portal](https://portal.azure.com/) and log in with your Azure Free Trial credentials.

2. **Create a Resource Group**  
   - On the left sidebar, click **Resource groups**.
   - At the top of the page, click **+ Create**.
   - **Fill in the details**:
     - **Subscription**: Ensure **Free Trial** is selected.
     - **Resource Group Name**: Enter a name (e.g., `myResourceGroup`).
     - **Region**: Choose a region (e.g., **East US**).
   - Click **Review + Create**, then click **Create**.

   Your resource group will now be created and will appear in the list of **Resource Groups**.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Step 2: Create a Windows Virtual Machine (VM)**

1. **Navigate to Virtual Machines**  
   On the left sidebar of the Azure Portal, click **Virtual Machines**.

2. **Create a Virtual Machine**  
   - Click **+ Create** and then **+ Virtual Machine**.

3. **Basic Information for the VM**  
   - **Subscription**: Ensure **Free Trial** is selected.
   - **Resource Group**: Select the resource group you just created (e.g., `myResourceGroup`).
   - **VM Name**: Choose a name for your VM (e.g., `myWindowsVM`).
   - **Region**: Select the region (e.g., **East US**).
   - **Availability Options**: Select **No infrastructure redundancy required** (for simplicity).
   - **Image**: Choose **Windows Server 2019 Datacenter** (or another Windows version).
   - **Size**: Click **Change size** and select **B1s** (eligible for free trial usage).
     - The **B1s** VM is eligible for free use in the Azure Free Trial for 12 months. It has 1 vCPU and 1 GB of RAM.
   - **Authentication Type**: Choose **Password**.
     - **Username**: Enter a username (e.g., `adminuser`).
     - **Password**: Enter a strong password and confirm it (e.g., `YourStrongPassword123!`).
     - --------------- USERNAME : AdminUser ---------------------
    ----------- PASSWORD : Ct@#9912088878 -----------------
   - **Public Inbound Ports**: Choose **Allow selected ports** and select **RDP (3389)** for Remote Desktop access.

4. **Disk Options**  
   - **OS Disk Type**: Keep the default **Standard HDD** (you can change it later if needed).
   - Click **Next** to proceed.

5. **Networking Settings**  
   - The default network settings should work for basic deployment. Ensure that the **Virtual Network** is created automatically.
   - **Public IP**: Ensure a **Public IP** is assigned to the VM (this is necessary for RDP access).
   - **Network Security Group (NSG)**: Ensure the NSG is configured to allow **RDP (3389)**.

6. **Review and Create**  
   - Review all settings to ensure they are correct.
   - Click **Create** to begin the deployment of the VM.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Step 3: Monitor Deployment and Get the Public IP Address**

1. **Deployment Progress**  
   After clicking **Create**, Azure will start provisioning your VM. This may take a few minutes. You can monitor the deployment in the **Notifications** area of the portal.

2. **Get the Public IP Address**  
   - Once the deployment is complete, go to the **Overview** page of your newly created VM.
   - Find the **Public IP Address** in the Overview section. This is the IP address you'll use to connect to your VM using RDP.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Step 4: Connect to the VM Using RDP**

1. **Open Remote Desktop Connection (RDP)**  
   - On your local computer, search for **Remote Desktop Connection** (on Windows, press the **Windows key** and type “Remote Desktop Connection”).
   
2. **Enter the Public IP Address**  
   - In the RDP client, enter the **Public IP Address** you obtained from the VM's Overview page.
   - Click **Connect**.

3. **Enter Credentials**  
   - When prompted, enter the **username** and **password** you created when setting up the VM (e.g., `adminuser` and `YourStrongPassword123!`).

4. **Access Your VM**  
   - You should now be connected to your Windows VM via RDP.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Step 5: Monitor Usage and Resource Limits**

1. **Check Azure Usage**  
   - Go to the **Cost Management + Billing** section in the Azure portal.
   - Monitor your **remaining credits** and usage for the **Azure Free Trial** subscription.

2. **Free Services**  
   - Some services, like the **B1s VM**, are free for the first 12 months. Be sure to track your usage and avoid going over the monthly free limits.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Important Notes for Azure Free Trial**

- **Limited Credit**: The Azure Free Trial gives you $200 in credits for the first 30 days. Once the credits are exhausted or after 30 days, you may need to upgrade to a pay-as-you-go subscription or you may lose access to some services.
- **VM Size**: The **B1s VM** is a low-cost VM that is eligible for free usage for the first 12 months of the Free Trial.
- **Resource Limits**: Be mindful of Azure Free Trial limits (e.g., the number of resources or total disk space) and monitor your usage to avoid charges.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### **Conclusion**
With these steps, you’ve successfully created a **Resource Group** and a **Windows Virtual Machine (VM)** using your **Azure Free Trial** subscription. You can now access the VM using RDP and start testing or using your Azure environment.

Let me know if you need any further help!
