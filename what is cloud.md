###  what is cloud ?

10 or 15 years back we don't have any cloud providers , companies like google used procure some servers to run their applications .
server is nothing but a computer which have cpu+Memory+RAM to run processes and applications .
all servers are places in racks , and all the racks are placed in one room and data centers have multiple rooms like this.

each data center is called a availability zone , one region have upto 3 availability zones , and one country may have multiple regions.
each AD is isolated from each other , they won't share any power or network connection together .
while choosing the region consider from which location you application will get more requests and is there any data restriction in your region .
companies own data centers also called as on-primises or private cloud
Companies used to have system admins who will create abd maintain these servers , system admins used to monier and patch these servers continuously to remiduate the vulnarabilities .
They should have 24/7 power supply in order to run the applications continuously , the maintanance is also a overhead.

####  Typyes of cloud

there are mainly 3 types of cloud 

*  public
*  private
*  Hybrid


Amazon started AWS (Amazon web service) and established multiple data centers across the world .
AWS offers it will provide the requested servers to companies in requested regions , so that the companied no need to worry about the power supply and maintanance over head .
This whole concept is called public cloud .

still many companies like banking , finance and insurance use private cloud because of data prvacy andsecurity reasons .

if one company hosted their applications on public cloud and hostd their database on their own data center this concept is known as hybrid cloud (public+private)
if one company use some services from AWS and some services from Azure then this concept is known as multi cloud .

cloud computing is nothing but computing on cloud that means running the applications on cloud 


####  What is Virtualization :

Dividing one single physical server to multiple isolated servers with the help of hypervisor is called virtualization and the small small servers are called virtual servers .
All the public clouds use the same concepts and provide the virtual machines to requesters .
Each virtual machine has their own os ,cpu and memory and each machine feels like it is the real machine and unaware of the other machines .
If one VM is corrupted that doesn’t effect the other VM’s

####  Some terminology in cloud :

*  API
*  Scalability
*  Elasticity
*  High Availability
*  Fault Tolerance
*  Disaster Recovery
*  Latency
*  Availability Zones
*  Regions
*  Iaas
*  Paas
*  Saas
