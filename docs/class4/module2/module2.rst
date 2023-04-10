Module 2: App Connect 
========================================

.. image:: ../images/appconnect.png

**Narrative:** 
Everything has been running terrific at ACME with your current Network Connect model. Your boss is pleased with your work and has a new assignment for you. 
ACME has aquired a new company that utilizes Azure. None of their servers are public facing.

ACME wants to implement a globally available frontend that can serve content from either AWS or Azure. 
Inbound Internet traffic should always be sent to the AWS frontend with the Azure frontend acting as a backup for now.  

The on-prem backend server must be able to scan the private frontend in Azure on port 80. 
The frontend server in Azure WILL NOT have a public IP. ACME has truly gone multi-cloud!


**In Lab 3** we will be satisfying the latest ACME business requirements by providing a globally available frontend to the cloud application

**In Lab 4** we will solve the IP overlap problem introduced by the Azure acquisition by deploying App Connect and a site mesh group

**In Lab 5** we are offering a bonus application routing lab where requests from the backend server will be routed to AWS or Azure frontend based on URI. 

.. toctree::
   :maxdepth: 1
   :glob:

   lab*
