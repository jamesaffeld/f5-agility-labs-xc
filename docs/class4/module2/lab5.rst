Lab 5: Bonus Lab - L7 App Routing & Security 
==============================================

**Objective:**

*Configure the Global Frontend to perform Layer 7 routing.

*Configure security policy to protect the frontends from manual and automated web attacks.  

*Test connectivity and review application security events in the XC console.

.. image:: ../images/lab5bizreq.png

**Narrative:** 
Much like "The Real World", the requirements never stop coming. Now, ACME has 2 new deliverables for you to figure out. 

**First**, a new API has been added to the cloud frontends and will require Layer 7 routing at the global frontend in XC. 
The requirement is for any requests that have **/aws** in the URI should be routed to AWS. 
Any requests with **/azure** should be routed to Azure. 

**Second**, ever since exposing the frontends globally, they have noticed alot of automated aka bot traffic coming in to their application. 
They have asked if there is a way to apply security policy to identify and remediate the bots as well as manual attacks. 

|

.. image:: ../images/lab5.png

|

L7 App Routing
---------------

Adding Layer 7 App Routing with F5 Distributed Cloud is a simple task. 

In the **Side menu** under **Manage** click on **Load Balancers** >> **HTTP Load Balancers** and click on the **3 Buttons** under the **Actions** menu for your **animal-name-acme-frontend**.

Click **Manage Configuration** and then **Edit Configuration** in the top right. 

|

.. image:: ../images/lab5mg.png

|

Scroll down to where you see **Routes** and click the blue hyperlink "**Configure**"

|

.. image:: ../images/routes.png

|

Click **Add Item**

Enter the following values:

==================================      ==============
Variable                                Value
==================================      ==============
Route Type                              Simple Route
HTTP Method                             GET
Path Match                     HTTP
Headers        **uncheck**
Origin Pools                              80
Host Rewrite Method                            See Below 
==================================      ==============



















Sanity Check
-------------
**This is what you just deployed.**

Thank you for completing the lab!


