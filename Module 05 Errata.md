# AZ-700T00 Designing and Implementing Microsoft Azure Networking Solutions - Module 05 Errata

## Module 05 – Load balance HTTP(S) traffic in Azure (Total Time ~55 Minutes)

### Exercise: Deploy Azure Application Gateway (~25 Min)

Task 1:  Create an application gateway <br>

### Prior to creating the Application Gateway you will need to create the Virtual Netowrk.  As the interface has changed and no longer allows you to create more than 1 subnet during the creation of the Gateway. <br>

Use the following steps to create the Virtual network  <br>
1. Search for Virtual network  <br>
2. Create <br>
3. Create Resource Group:  ContosoResourceGroup <br>
4. Name:  ContosoVNet <br>
5. Change default subnet name to AGSubnet <br>
6: Add Subnet <br>
name: BackendSubnet <br>
address range: 10.0.1.0/24 <br>
Review and create > Create <br>

Return to Task 1 Step 1 - when asked about the network configuration choose the networks you just created <br>
Step 4:  Resource Group:  Choose ContosoResourceGroup <br>
Virtual Network: ContosoVNet <br>
Subnet:  ASGSubnet <br>

You will need to give the Application Gateway a Priority when configuring the listener.  Set it to 100 <br>

Task 2:  Create virtual machines <br>
Step 1:  if prompted use advance setting to create a storage account <br>

### Exercise: Create a Front Door for a highly available web application using the Azure portal (~30 Min)

If during the creation you get a quota error - close the creation window - restart the creation- choose a different region <br>
Unique default hostname (preview) on - Slide the bar to the left <br>
