# AZ-700T00 Designing and Implementing Microsft Azure Networking Solutions  - Module 06 Errata

## Module 06 – Design and implement network security (Total time ~135 Minutes)

### Exercise:Configure DDoS Protection on a virtual network using the Azure portal (~40 Min)

Task 4: Configure DDoS telemetry <br>
Step 4: Name must be all lowercase <br>

Task 6: Configure DDos Alerts <br>
Step 3: You will need to select all images the in the Marketplace choose the correct image <br>
Step 3: You will need to select all sizes, you may have to search for the B1ls size <br>
Step 7: After downloading the key, select return to creating virtual machine <br>

Configure DDoS alerts <br>
Step 12: Click Next: Actions <br>
Step 13: Click Details Then Fill in the information > click tags <br>

Task 7: Submit a DDoS service request to run a DDoS attack <br>
Step 1: When creating the breakingpoint account you will need to use a valid email address that you have access to (Recommend creating a dummy outlook account) <br>
NOTE - You will not be able to actually schedule the DDoS attack as you are not a Global Admin in the Cloud Slice version of the lab <br>

Task 8: Clean up resources <br>
Step 1: if prompted create a storage account <br>

### Exercise: Deploy and configure Azure Firewall using the Azure portal (~60 Min)

Task 2: Create a virtual network and subnets <br>
Step 7: Add a third subnet. In the subnet purpose drop down choose Firewall Management (Forced tunneling) <br>
This will create a subnet call AzureFirewallManagementSubnet > change Starting address to 10.0.3.0/26 <br>

Task 4: Deploy the firewall and firewall policy <br>
Step 1: Use the Search resources box at the top of the Azure portal instead of create a resource <br>
In step 3: Clear checkbox from Enable Firewall Management NIC

Task 6: Configure an application rule <br>
Wait until the Application rule has deployed before proceeding<br>

Task 7: Configure a network rule <br>
Wait until the Network rule has deployed before proceeding<br>

Task 8: Configure a Destination NAT (DNAT) rule <br>
Wait until the DNAT rule has deployed before proceeding<br>

### Exercise: Secure your virtual hub using Azure Firewall Manager (-35 Min)

Task 2: Create the secured virtual hub <br>
Step 3: Under Deployments, select Virtual Hubs <br>

Task 4: Deploy the servers <br>
Wait until the Task 3 completes <br>

Task 5: Create a firewall policy and secure your hub <br>
Step 2: Under Security, select Azure Firewall Policies <br>

Task 6: Associate the firewall policy <br>
Wait for Task 5 to complete before moving on <br>
Step 4: Manage associations is located on the top bar <br>
Association took over 15 minutes <br>

