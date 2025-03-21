# AZ-700T00 Designing and Implementing Microsoft Azure Networking Solutions  - Module 04 Errata

## Module 04 -Load balance non-HTTP(S) traffic in Azure (Total time ~60 Minutes)

### Exercise: Create and configure an Azure load balancer (~60 Min)

Task 1: Create the virtual network <br>
Step 3: Delete the existing Virtual Network <br>
Wait for the deployment to complete before moving on <br>

Task 2: Create backend servers <br>
Step 1: If prompted use advance setting to create a storage account <br>
Use existing Resource Group <br>
Step 2: path to files  F:\allfiles\exercises\M04 <br>
Step 3: Once VM2 is created you may have to hit enter for the last cmdlet to run.  Do not close the Cloud Shell until the  all VMs are created <br>

Task 4: Create load balancer resources <br>
Do not continue until all VMs are created from task 2 <br>
Create a backend pool and add VMs to the backend pool <br>
Step 4: Click Add under IP configuration to add Virtual Machines <br>
Step 6: Click Save <br>

Create a health probe <br>
Step 2: Unhealthy threshold has been removed <br>

Task 5: Test the load balancer <br>
Create test VM <br>
Step 2: Leave the size that is auto filled <br>

### Exercise: Create a Traffic Manager profile using the Azure portal

Task 1: Create the web apps <br>
If during the creation you get a quota error - close the creation window - restart the creation- choose a different region <br>
Step 2 and step 7: Unique default hostname (preview) on - Slide the bar to the left <br>
