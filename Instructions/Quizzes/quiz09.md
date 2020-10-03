## Quiz 9

1\. You plan to create an Azure Web App in the East US region. You need to ensure that this web app scales out with demand, to prevent downtime. You also need to ensure that the data that resides inside of the application will remain secure and never become exposed to anyone outside of the organization. Which App Service plan SKU will you chose that will meet these requirements and also save on cost?

A  FREE

B  B1

C  SHARED

D  I1

2\. You have a subscription named Subscription1. You create a new Azure VM in your subscription named VM5 running Windows 2012 R2. You try to connect and login to VM5, but you get an error that says "We couldn't connect to the remote PC. Make sure the PC is turned on and connected to the network, and that remote access is enabled." You have verified that VM5 is running and has been assigned a public IP address. What change do you need to make in order to successfully connect and login to VM5?

A  Add a rule to the Network Security Group that will allow port 3389

B  Select Reset password from the VM blade

C  Use Network Watcher for detailed connection tracing

D  You need to access the VM from a computer that's in the same subnet


3\. You have an Azure subscription that contains the following Virtual Machine Scale Set named myScaleSet:

You need to remove instance id 5 from the virtual machine scale set. Which command should you use?

A  Remove-AzVmssVMDataDisk -VM $VirtualMachine -Lun 0

B  Remove-AzVmss -ResourceGroupName "Group001" -VMScaleSetName "VMScaleSet001"

C  az scale set remove --instance-ids 3 --name MyScaleSet\_5 --resource-group MyRG

D  az vmss deallocate --instance-ids 3 --name MyScaleSet --resource-group MyRG

4\. You have created a new Azure virtual machine named VM1. You plan to use VM1 as a web server, which will require the VM to be accessible using HTTPS protocol. A Network Security Group (NSG) is attached to the NIC of VM1 with the following rules:
What changes do you have to make to the NSG in order to meet the requirements for VM1?

A  Change the priority of CustomRule5 to 601

B  Change the priority of CustomRule4 to 200

C  Change the port of CustomRule5 to 443 only

D  Change the priority of CustomRule3 to 200

5\. VM1 is a D-series Linux virtual machine in an availability set, which has availability across two fault domains and five update domains. VM1 experiences a hardware failure, but the memory is preserved and doesn't require a reboot. What will happen to the VM when this event occurs?

A  Since the memory is preserved, the VM will migrate to all new hardware, except for the memory component

B  The VM will be decommissioned and a support ticket will be automatically generated. You will have to call support in order to retrieve the data from your VM

C  Azure will keep the VM running on the same hardware because fault domains are in place for the VM

D  Azure will migrate VM1 from failing hardware to a healthy physical host and the VM will be paused for up to five seconds

6\. You have an Azure subscription named Subscription1. In Subscription1, you have an Azure virtual machine named VM1. Attached to VM1 are two network interface cards. You require a third network interface card with a network bandwidth above 1000 Mbps for your storage area network. What should you do?

A  Create an additional VM in the same subnet and connect to VM1 over the LAN

B  Create a new subnet with a sufficient number of available IP addresses

C  Create a new storage account to store data for VM1

D  Change the VM SKU to Standard\_A4 or larger

7\. You have an Azure Kubernetes Service (AKS) cluster named AKS1 within the resource group named RG1. You are trying run the command kubectl get all from the Azure Cloud Shell ([https://shell.azure.com](https://shell.azure.com)) to view your cluster resources. You received the error Error from server (BadRequest): the server rejected our request for an unknown reason. You've verified that the resources exist and the command is correct. What do you need to do in order to view your cluster resources from the Azure Cloud Shell?

A  Retrieve the access credentials using the command az aks get-credentials --name AKS1 --resource-group RG1

B  Log into the cluster GUI from the Azure Portal

C  Install the kubectl tool

D  Access the Kubernetes Dashboard using the command az aks browse --name AKS1 --resource-group RG1

8\. VM1 is located in the West US region, and the OS disk is Premium SSD. The size of VM1 is currently Standard\_D2s\_v3, but you need to change the size to Standard\_D2. You are able to select the size from the size blade, but you receive an error message. Why can't you change the VM size?

A  You need to provide the username and password for the OS to upgrade

B  Standard\_D2 does not support premium SSD disks

C  The size Standard\_D2 is not available in the West US region

D  You did not shut down (deallocated) VM1 before you change the size

9\. Subscription1 contains an Azure VM named VM1. You have added a data disk to VM1, as well as a new network interface card. You need to create two more Azure VMs just like this one named VM2 and VM3. What is the most efficient way to create VM2 and VM3 that will minimize cost?

A  Backup the VM and recover to a different region

B  Redeploy VM1 with the new disk and NIC and deploy the template to VM2 and VM3

C  Select Export template from VM1 blade, then deploy VM2 and VM3 with that template

D  Create an image from VM1 and use the image to deploy VM2 and VM3

10\. You are trying to create a new Azure Kubernetes Service (AKS) cluster from your local workstation. The AKS cluster must contain three nodes and ensure access to the worker nodes in order to troubleshoot the kubelet. You have authenticated to Azure from your local workstation with the Azure CLI. What command will you use to create an AKS cluster named AKS1 with the necessary components inside of the resource group named RG1?

A  az aks create -g RG1 -n AKS1 --generate-ssh-keys --node-count 3

B  az kubernetes create --name AKS1 --group RG1 --nodes 3 --generate-keys

C  az aks create --name AKS1 --resource-group RG1 --nodes 3 --ssh-key-value \~/.ssh/id\_rsa.pub

D  az kubernetes create --name AKS1 --resource-group RG1 --nodes 3 --generate-keys

11\. You have created an application that is to be run on Linux containers named ContainerApp1. You've created an Azure container instance with an FQDN, but you notice that when the container restarts, all application data is lost. What is the best solution to preserve the data associated with your application?

A  Create a public blob storage container and share the URI with the application

B  Create a storage account and share the SAS with the application

C  Mount an Azure file share as a volume in Azure Container Instances

D  Run the container on a VM, and use the managed disk attached to the VM

12\. VM1 is located in the East US region. You have added a premium SSD data disk to VM1, but the IOPS are not satisfying the needs of your application, how can you change the speed of the disk?

A  Select the disk configuration and increase the size

B  Shut down (Deallocate) the VM

C  Export the disk and convert to VHD

D  Create a new disk and migrate the data

13\. You've created a Dockerfile that contains the necessary steps to build an image that you plan to use for your application running as a Web App in App Services named APP1. You have created an Azure Container Registry, which is where you plan to store your images to be used for APP1. What should your next step be?

A Run the az acr build command

B Create the App Service Plan

C Run the docker push command

D Run the docker login command

14\. You have an Azure subscription named Subscription1. You have created a web app named App1 in Subscription1 that is sourced from a git repository named Git1. You need to ensure that every commit to the master branch in Git1 triggers a deployment to a test version of the application before releasing it to production. What are two changes that you must make to App1 to fulfill this requirement?

A  Create a build server with the master branch of Git1 as the trigger

B  Configure custom domains for test and production versions of App1

C  Add a new deployment slot to App1 to release the test version of App1

D  Create a new web app and configure failover settings from test to production

15\. Subscription1 contains an Azure VM named VM1 with the following configuration:

•	VM Size: Standard\_D2s\_v3
•	Public IP Address: 52.173.36.55
•	Resource Group: RG1
•	Availability Zone: None
•	Location: Japan East
•	Disk Type: Standard HDD

What are two things you can do to reduce data loss and achieve a 99.9% SLA?

A  Create a recovery services vault and enable replication for VM1

B  Move VM1 to a paired region

C  Place the VM in an availability zone

D  Change the disk type to Premium SSD


Answers: (1) D  (2) A (3) D (4) A, D (5) D (6) D (7)  A (8)  B (9) C (10) A (11) C (12) A, B (13) A (14)  A,C (15) A, D