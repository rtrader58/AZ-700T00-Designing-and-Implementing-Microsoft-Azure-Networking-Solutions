# AZ-700T00 Designing and Implementing Microsft Azure Networking Solutions  - Errata All Modules<br>
 
## Module 01 – Introduction to Azure virtual networks (Total Time ~70 Minutes)

### Exercise: Design and implement a Virtual Network in Azure (~25 Min) 

### Required Lab Setup

Prepare cloud shell for later use <br>
Step 5:  Use the resource group that is auto populated <br>

When creating the virtual networks delete the existing IP range <br>

### Exercise: Configure DNS settings in Azure ( ~25 Min) 

Task 4: Verify records are present in the DNS zone <br>
Exercise - Connect to the Test VMs using RDP <br>
After step 19 disconnect from both RDP sessions <br>

### Exercise: Connect two Azure Virtual Networks using global virtual network peering (~20 Min) 

No errata

## Module 02 – Design and implement an identity hybrid networking (Total Time ~135 Minutes)

### Exercise: Create and configure a virtual network gateway (~70 Min) 

Task 1:  Create CoreservicesVnet and ManufacturingVnet <br>
Step 1:  If required use advanced settings to create a storage account <br>

Task 3: Create ManufacturingVM  <br>
Step 2: If creating the Manufacturing VM fails, open the ManufacturingVMazuredeploy.parameters.json - change the VM size from D2as_v5 to DS1_v2 > save the file then upload <br>

# Complete tasks 6 and 7 before taking a break 

Task 6: Create CoreServicesVnet Gateway <br>
Before Step 1:  The GatewaySubnet does not get created using the JSON use the following steps to create the subnet <br>
Search for Virtual Network > Select ManufacturingVnet > Select Subnets under Settings> Select + Gateway Subnet > Starting address 10.30.0.0 > Size /27 > Add <br>

Step 3:  If Public IP Address Type is greyed out continue <br>
Continue with Task 7 while Gateway is being built. <br>

Task 7: Create ManufacturingVnet Gateway <br>
Step 3:  If Public IP Address Type is greyed out continue <br>
Routinely click in the Azure Portal so the lab does not end on you <br>
Both Virtual Gateways have to finish building before continuing to Task 8 <br>

Task 10: Verify that the connections connect <br>
Step 2:  it took 10 minutes after gateways were finished building before status showed connected <br>

### Exercise: Create a Virtual WAN by using Azure Portal (~65 Min)

No errata <br>

## Module 03 – Design and Implement Azure ExpressRoute (Total time ~75 Minutes)

Throughout the lab use the search box to search for ExpressRoute Circuits <br>

### Lab Setup

Prepare cloud shell for later use <br>
Step 5:  Use the existing Resource Group <br>

### Exercise: Configure an ExpressRoute Gateway (~60 Min)

Task 1: Create the VNet and gateway subnet <br>
Delete the 10.0.0.0 Virtual Network <br>

Step 5:   After pasting delete the /16 <br>
Subnet size:  /16 <br>

Step 6:  Select Virtual Network Gateway in the Subnet template dropdown <br>
Starting address:  After pasting delete the /27 <br>
Subnet size:  choose /27 <br>

Task 2: Create the virtual network gateway <br>

Step 3:  Resource Group will auto populate
 <br>

### Exercise: Provision an ExpressRoute circuit (~15 Min)

Task 1: Create and provision an ExpressRoute circuit <br>
Step 1:  If ExpressRoute is not an option search for it <br>

Task 2: Retrieve your Service key <br>
If ExpressRoute does not appear - search for ExpressRoute Circuit <br>

Task 4: Clean up resources <br>

When cleaning up the lab you will need to create a storage account, use advanced setting to create the storage account <br>

## Module 04 - Load balance non-HTTP(S) traffic in Azure (Total time ~60 Minutes)

### Exercise: Create and configure an Azure load balancer (~60 Min)

Task 1: Create the virtual network <br>
Step 3:  Delete the existing Virtual Network <br>
Wait for the deployment to complete before moving on <br>

Task 2:  Create backend servers <br>
Step 1:  If prompted use advance setting to create a storage account <br>
Use existing Resource Group <br>
Step 2:  path to files  F:\allfiles\exercises\M04 <br>
Step 3:  Once VM2 is created you may have to hit enter for the last cmdlet to run.  Do not close the Cloud Shell until the  all VMs are created <br>

Task 4: Create load balancer resources <br>
Do not continue until all VMs are created from task 2 <br>
Create a backend pool and add VMs to the backend pool <br>
Step 4:  Click Add under IP configuration to add Virtual Machines <br>
Step 6:  Click Save <br>

Create a health probe <br>
Step 2:  Unhealthy threshold has been removed <br>

Task 5: Test the load balancer <br>
Create test VM <br>
Step 2:  Leave the size that is auto filled <br>

## Module 05 – Load balance HTTP(S) traffic in Azure (Total Time ~55 Minutes)

### Exercise: Deploy Azure Application Gateway (~25 Min)

Task 1:  Create an application gateway <br>

### Prior to creating the Application Gateway you will need to create the Virtual Netowrk.  As the interface has changed and no longer allows you to create more than 1 subnet during the creation of the Gateway. <br>

Use the following steps to create the Virtual network  <br>
1. Search for Virtual network  <br>
2. Create <br>
3. Create Resource Group:  ContosoAppGateway <br>
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

No errata <br>

## Module 06 – Design and implement network security (Total time ~135 Minutes)

### Exercise: Configure DDoS Protection on a virtual network using the Azure portal (~40 Min)

Task 4: Configure DDoS telemetry <br>
Step 4:  Name must be all lowercase <br>

Task 6:  Configure DDos Alerts <br>
Step 3:  You will need to select all images the in the Marketplace choose the correct image <br>
Step 3:  You will need to select all sizes, you may have to search for the B1ls size <br>
Step 7:  After downloading the key, select return to creating virtual machine <br>

Configure DDoS alerts <br>
Step 12:  Click Next: Actions <br>
Step 13:  Click Details Then Fill in the information > click tags <br>

Task 7:  Submit a DDoS service request to run a DDoS attack <br>
Step 1:  When creating the breakingpoint account you will need to use a valid email address that you have access to (Recommend creating a dummy outlook account) <br>

Task 8:  Clean up resources <br>
Step 1:  if prompted create a storage account <br>

### Exercise: Deploy and configure Azure Firewall using the Azure portal (~60 Min)

Task 4: Deploy the firewall and firewall policy <br>
Step 1:  Use the Search resources box at the top of the Azure portal instead of create a resource <br>

Task 7:  Configure a network rule <br>
Wait until the Application rule has deployed <br>

Task 8:  Configure a Destination NAT (DNAT) rule <br>
Wait until the Network rule has deployed <br>

### Exercise: Secure your virtual hub using Azure Firewall Manager (-35 Min)

Task 2:  Create the secured virtual hub <br>
Step 3:  Under Deployments, select Virtual Hubs <br>

Task 4: Deploy the servers <br>
Wait until the Task 3 completes <br>

Task 5:  Create a firewall policy and secure your hub <br>
Step 2:  Under Security, select Azure Firewall Policies <br>

Task 6:  Associate the firewall policy <br>
Wait for Task 5 to complete before moving on <br>
Step 4:  Manage associations is located on the top bar <br>

Association took over 15 minutes <br>

## Module 07 – Design and implement private access to Azure services (Total time ~ 80 Minutes)

### Exercise: Restrict network access to PAAS resources with virtual network service endpoints (~35 Min)

Task 4:  Add additional outbound rules <br>
Step 2:  Enter Any for the source <br>

Task 5:  Allow access for RDP connections <br>
Step 3:  Choose Any for Destination <br>

Task 7: Create a file share in the storage account <br>
Step 1:  Option to searching is to Go to resource after completion <br>

Task 8: Restrict network access to a subnet <br>
Step 2:  Select Enable from selected networks and IP addresses <br>
Step 8:  Copy the key to notepad <br>

Task 9: Create virtual machines <br>
Step 1:  Create a Storage account if needed <br>

### Exercise: Create an Azure Private Endpoint using Azure PowerShell (~45 Min)

Task 2: Create a virtual network and bastion host <br>
Note:  It took ~20 Minutes to deploy the Bastion <br>

Task 3: Create a test virtual machine <br>
Copy the script into notepad <br>
Either copy / paste or type the $Cred command <br>
When prompted enter the credentials <br>

Student <br>
Pa55w.rd1234 <br>

Copy and paste the remaining script into the cloud shell <br>

## Module 08: Design and implement network monitoring (Total time ~55 Minutes)

### Exercise: Monitor a load balancer resource using Azure Monitor (~55 Min)

Task 3: Create a backend pool <br>
Step 4: click save <br>

Task 4: Create a health probe <br>
Step 1: From the myIntLoadBalancer page of your load balancer, under Settings, click Health probes, then click Add. <br>
Step 2:  On the Add health probe page, enter the information from the table below.  Ignore Unhealthy Threshold Setting <br>

Task 5: Create a load balancer rule <br>
Step 1: From the myIntLoadBalancer page of your load balancer, under Settings, click Load balancing rules, then click Add. <br>

Task 6: Create backend servers <br>
Step 1:  if prompted create a storage account <br>

Task 7: Add VMs to the backend pool <br>
Step 3:  Under IP configuration select +Add <br>

Task 8: Install IIS on the VMs <br>
Step 5:  Select the Popup blocker on the address bar choose to allow and select done <br>

Click Connect <br>

Task 9: Test the load balancer <br>
Connect to the test VM to test the load balancer <br>
Step 10:  Click on Edge icon in the task bar to open the web browser <br>

Task 13: View resource health <br>
Step 1:  Search for Monitor if not shown <br> 
