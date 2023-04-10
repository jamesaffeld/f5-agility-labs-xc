Lab 3: Globally Available Front End 
================================================


**Narrative:**


Everything has been running terrific at ACME with your current Network Connect model. Your boss is pleased with your work
and has a new assignment for you. ACME has aquired a new company that utilizes Azure. None of their servers are public facing. 


ACME wants to implement a globally available frontend in Azure. Inbound Internet traffic should always be sent to the AWS frontend with the Azure frontend acting as a backup. 
The on-prem backend server must be able to scan the private frontend in Azure on port 80. The frontend server in Azure WILL NOT have a public IP. 
ACME has truly gone multi-cloud! 

**What they want:**

.. image:: ../images/lab3bizreq.png

Unfortunately, after doing your due diligence, you find that the Azure VNET overlaps with the AWS subnets. You think to yourself, this is going to be tricky, and reach out to your trusted F5 Solutions Engineer to see how this will work with Network Connect. 


Your F5 Solutions Engineer explains that IP overlap between sites is a common problem and one that can be easily solved with Distributed Cloud App Connect. 
App Connect alleviates this problem by leveraging the XC Nodes as Software Defined proxies rather than SD Routers as they were configured with Network Connect.   


After reviewing the architecture with you, your Solutions Engineer advises you to break up these requirements in to 2 specific deliverables. 

**Deliverable 1**
Create a globally scaled and future-proof frontend with the XC Regional Edges **(Lab 3)**

.. image:: ../images/lab3.png


**Deliverable 2**
Leverage App Connect to create a site mesh which will allow for secure site to site connectivity regardless of IP overlap. **(Lab 4)**

.. image:: ../images/lab4.png


Regional Edge
~~~~~~~~~~~~~

A Regional Edge (RE) is part of Distributed Cloud Global Network that provides connectivity 
to services.  Previously when we deployed the UDF / AWS sites these were considered
"Customer Edge (CE)" and they make use of RE to communicate (each CE is associated with 
two RE).



















 










 









