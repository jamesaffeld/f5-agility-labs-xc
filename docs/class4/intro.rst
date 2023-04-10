Introduction to the Lab
=======================

**Narrative:**

Congratulations! You are a Network Engineer at ACME company. 


ACME has an Application team that supports internally developed traditional and modern apps, vendor provided and SAAS applications. 
They have started utilizing some public cloud (AWS) IAAS for several applications and have come to you with a new requirement that an on-prem backend server must be able to securely communicate
with the AWS workloads over a secure connection. For lab simplicity the backend (on-prem) is a pretend security device in this exercise, and needs to scan the AWS workload on port 80. 
It could just as easily be thought of as a API to API or frontend to backend. Other backends or frontends may be added in the future.  

As the Network Engineer you are tasked with evaluating how you will securely connect the on-prem network to the AWS network. 
At first you consider the classic methods of deploying and managing your own IP-SEC solution but realize that this will be complex and costly.

You recently saw a post on LinkedIn about a SAAS product that F5 has, claiming to solve multi-cloud network complexities. 
Given your current predicament and industry knowledge of F5 being a leader for decades, you decide to check it out and end up in the chair you are sitting in today, taking a first-hand look at how F5 makes Multi-Cloud Networking (MCN) simple and secure. 

.. Note:: The requirements start out simply enough but will get progressively more "Real World" as the labs progress.

**Before Cloud Migration**

.. image:: ./images/pre-migration.png


**Intended design after Cloud Migration**

.. image:: ./images/post-migration.png


**Your job, should you choose to accept it, and not get demoted, is to figure out the best way for the backend system to privately communicate with the frontend server.**


Lab Environment
---------------

The on-prem environment is emulated by the F5 UDF environment and contains an Ubuntu Server and an XC Node. 

The AWS cloud environment contains a prebuilt XC Node and a workload hosting a web frontend.  **You will not have access to the AWS console.**

The Azure cloud environment contains a prebuilt XC Node and a workload hosting a web frontend.  **You will not have access to the Azure console.**

.. Important:: While we are keeping the labs intentionally simple today with just a single on-prem DC and 2 Cloud sites, F5 Distributed Cloud supports much more advanced use-cases. 

.. toctree::
   :maxdepth: 1
   :glob:

