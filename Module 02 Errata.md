# AZ-700T00 Designing and Implementing Microsoft Azure Networking Solutions - Module 02 Errata

## Module 02 – Design and implement an identity hybrid networking (Total Time ~135 Minutes)

### Exercise: Create and configure a virtual network gateway (~70 Min) 

Task 1: Create CoreservicesVnet and ManufacturingVnet <br>
Step 1: If required use advanced settings to create a storage account <br>

Task 3: Create ManufacturingVM  <br>
Step 2: If creating the Manufacturing VM fails, open the ManufacturingVMazuredeploy.parameters.json - change the VM size from D2as_v5 to DS1_v2 > save the file then upload <br>

# Complete tasks 6 and 7 before taking a break 

Task 6: Create CoreServicesVnet Gateway <br>
Step 3: If Public IP Address Type is greyed out continue <br>
Continue with Task 7 while Gateway is being built. <br>

Task 7: Create ManufacturingVnet Gateway <br>
Before Step 1:  The GatewaySubnet does not get created using the JSON use the following steps to create the subnet <br>
Search for Virtual Network > Select ManufacturingVnet > Select Subnets under Settings> Select + Gateway Subnet > Starting address 10.30.0.0 > Size /27 > Add <br>

Step 3: If Public IP Address Type is greyed out continue <br>
Routinely click in the Azure Portal so the lab does not end on you <br>
Both Virtual Gateways have to finish building before continuing to Task 8 <br>

Task 10: Verify that the connections connect <br>
Step 2: it took 10 minutes after gateways were finished building before status showed connected <br>

### Exercise: Create a Virtual WAN by using Azure Portal (~65 Min)

No errata <br>
