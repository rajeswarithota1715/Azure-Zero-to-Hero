What is resource, resource manager and resource group:
Whatever you create by using the Azure service is a resource , whether it’s a VM or storage calls or something else .
There is a interface called Resource manager which acts as a mediator between user and actual resource .
RM will evaluate the user request and responsible for creating the resources accordingly .
Every resource should be associated with one resource group
Each resource can be associate with only one resource group
We can group all the resources related to same project under one resource group , this way we can easily manage billing , auditing and access 
