<div align="center">
<img width="595" height="335" alt="Microsoft Azure"  src="https://github.com/user-attachments/assets/3a88a6f6-e886-407c-8860-9651406fa180" />
</div>
# Configuring a Virtual Machine and Connecting to the Remote Desktop in Azure
This Tutorial we will have to create, edit and connect to a Virtual Machine (Remote Desktop).

## Technologies Used
- Microsoft Azure
- Remote Desktop Connection or the Windows app for Mac


## Part 1: Creating a Resource Group

A Resource Group acts as a logical container for all the assets you will create for this lab.

1.  **Search for Virtual Machines**: Open the Azure portal and use the top search bar to find "Virtual machines".
    
2.  **Start Creation**: Click **Create** and then select **Azure virtual machine**.
    
3.  **Define the Group**: Under the **Project details** section, look for the **Resource group** field.
    
4.  **Create New**: Click the **Create new** link directly below the dropdown menu.
    
5.  **Name and Save**: Type a name for your group (e.g., `osTicket-Lab`) and click **OK**.
    


## Part 2: Configuring the Virtual Machine

Once the resource group is defined, you can specify the hardware and operating system for your server.

### Instance Details

-   **Virtual Machine Name**: Enter `osTicketVM`.
    
-   **Region**: Select **(US) East US 2**.
    
    > **Note**: It is important to keep the region consistent across all related resources you create.
    
-   **Image**: Select **Windows 10 Pro/Enterprise, version 22H2**.
    

### Administrator Account

These credentials will be used later to log in via Remote Desktop:

-   **Username**: Enter `labuser`.
    
-   **Password**: Enter `osTicketPassword1!`
	>**Note**: Its never a good idea to post your username and password anywhere. 

## Part 3: Accessing the VM

After Azure finishes deploying the resource, you need to find its "address" to begin the installation.

1.  **Find the Public IP**: Navigate to your new virtual machine's **Overview** page and look for the **Public IP address** (e.g., `20.246.83.74`).
    
2.  **Connect via RDP**: Open the **Remote Desktop Connection** app on your physical computer.
    
3.  **Log In**: Enter the **Public IP**, click **Connect**, and use the `labuser` credentials you created in Part 2.
