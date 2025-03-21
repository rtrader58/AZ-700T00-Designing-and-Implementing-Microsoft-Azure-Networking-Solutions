# AZ-700T00 Designing and Implementing Microsft Azure Networking Solutions - Module 03 Errata

## Module 03 – Design and Implement Azure ExpressRoute (Total time ~75 Minutes)

Throughout the lab use the search box to search for ExpressRoute Circuits <br>

### Lab Setup

Prepare cloud shell for later use <br>
Step 5:  Use the existing Resource Group <br>

### Exercise:  Configure an ExpressRoute Gateway (~60 Min)

Task 1: Create the VNet and gateway subnet <br>
Delete the Default Subnet <br>

Step 6:  Select Virtual Network Gateway in the Subnet template dropdown <br>
Starting address:  After pasting delete the /27 <br>
Subnet size:  choose /27 <br>

Task 2: Create the virtual network gateway <br>

Step 3:  Resource Group will auto populate <br>
Public IP address SKU - choose Standard <br>

### Exercise: Provision an ExpressRoute circuit (~15 Min)

Task 1: Create and provision an ExpressRoute circuit <br>
Step 1: If ExpressRoute is not an option search for it <br>
Step 2 and 3: There now only 1 blade  <br> 
Choose Standard for Resiliency <br>
Populate the remaining fields from step 2 and 3 information <br>
The allow classis operation in the picture has been removed <br>

Task 2: Retrieve your Service key <br>
If ExpressRoute does not appear - search for ExpressRoute Circuit <br>

Task 4: Clean up resources <br>

When cleaning up the lab you will need to create a storage account, use advanced setting to create the storage account <br>
