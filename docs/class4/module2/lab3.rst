Lab 3: Globally Available Front End 
================================================
**Objective:**

*Use XC Regional Edges to provide future-proof, globally available frontend.

*XC frontend (RE) must be able to load balance the 2 cloud frontends. 

*Expose Azure private frontend without adding a public IP for the workload. 

*Always prefer the AWS frontend for ingress traffic. 

**What they want:**

.. image:: ../images/mod2bizreq.png

**Narrative:**

Unfortunately, after doing your due diligence, you find that the Azure VNET overlaps with the AWS subnets. To make matters worse, 
the Azure server is not associated with any public IP and there is a security directive in place to not have any workload servers in Azure associated with a public IP without a security device. 
Lately the site has been getting pounded with traffic and frontend security has become a hot topic at ACME. 
You think to yourself, this is going to be tricky, and reach out to your trusted F5 Solutions Engineer to see how this will work with Distributed Cloud. 

Your F5 Solutions Engineer explains that IP overlap between sites is a common problem and one that can be easily solved with Distributed Cloud App Connect. 
App Connect alleviates this problem by leveraging the XC Nodes as Software Defined proxies rather than SD Routers as they were configured with Network Connect.

Also, you are informed that by using F5 Distributed Cloud Regional Edges for the frontend workloads, you will have full proxy visibility and analytics for the client traffic so the Security team will be pleased. 

After reviewing the architecture with you, your Solutions Engineer advises you to break up these requirements in to 2 specific deliverables. 

**Deliverable 1:**

Create a globally scaled and future-proof frontend with the XC Regional Edges **(Lab 3)**

.. image:: ../images/lab3.png


**Deliverable 2:**

Leverage App Connect for secure site to site connectivity regardless of IP overlap. **(Lab 4)**

.. image:: ../images/lab4goal.png


[INSERT Step by Step Documentation]


Sanity Check
-------------
**This is what you just deployed.**



















 










 









