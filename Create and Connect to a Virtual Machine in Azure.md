**Create and Connect to a Virtual Machine in Azure**

**Introduction**

In this tutorial, we will go through the steps to create a virtual machine (VM) in Azure and connect to it using Microsoft Remote Desktop. This will allow you to run applications and services directly in the cloud.

**Prerequisites**

- An active Azure account.
- A resource group already set up. (See previous sections if you haven't set this up yet)
- Access to a computer with Microsoft Remote Desktop installed (available for Windows and macOS).

**Steps to Create and Connect to a Virtual Machine**

**Step 1: Create a Virtual Machine**

**Navigation**

- From the Azure portal's home screen, search for and select **Virtual machines**.
- Click on **+ Create** and then **+ Virtual machine** to start the creation process.

**Configuration**

- **Subscription**: Select the Azure subscription you are using.
- **Resource group**: Choose the resource group you created earlier.
- **Virtual machine name**: Enter a name for your VM.
- **Region**: Choose the region where your VM will be hosted. It's best to select the same region as your resource group.
- **Image**: Select an OS image (e.g., Windows Server 2019, Ubuntu 18.04 LTS) depending on your requirements.
- **Size**: Choose the size of the VM. Azure will suggest sizes based on the image you selected. You can also view all sizes and select one that meets your performance and budget needs.
- **Administrator account**: Set up a username and a password that will be used to access the VM.
- **Inbound port rules**: Choose to allow selected ports (e.g., RDP 3389 for Windows, SSH 22 for Linux) for remote access.

**Create**

- Click **Review + create** to review your settings.
- Once validation passes, click **Create** to deploy your VM.

**Step 2: Connect to Your Virtual Machine using Microsoft Remote Desktop**

**Find IP Address**

- Once the VM is created, go to the VM page in the Azure portal.
- Under the **Overview** tab, you'll find the public IP address. Copy this address.

**Connect Using Remote Desktop**

- Open Microsoft Remote Desktop.
- Click on **Add PC** or **Connect**, then enter the copied public IP address.
- Enter the username and password you set up when creating the VM.
- Click **Connect**.

**Additional Settings**

- If prompted, accept the certificate warning by clicking **Yes** or **Continue** to proceed.

**Conclusion**

You have successfully created a virtual machine in Azure and connected to it using Microsoft Remote Desktop. This setup allows you to manage and use your VM from anywhere, simulating a local desktop experience in the cloud.

