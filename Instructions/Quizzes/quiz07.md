## Quiz 07

1\. You have just created a General\-purpose V2 storage account in Azure\. From a VM located in your on\-prem environment\, you've logged into your Azure subscription using the Connect\-AzConnect command from the PowerShell command line\. Next\, you need to retrieve the key\, in order to access your storage account\. Which PowerShell cmdlet will you use to retrieve the access key?

A Get-AzStorageAccount

B Get-AzStorageContainerKey

C Get-AzStorageContainerStoredAccessPolicy

D Get-AzStorageAccountKey

2.You have data in an AWS S3 Bucket named myS3Bucket and you need to copy all of its contents to a container named container1 in an Azure storage account named consiliumdata. Which command would be most efficient use of getting the data from the S3 bucket to the Azure storage container?

A azcopy copy 'https://s3.amazonaws.com/myS3Bucket' 'https://consiliumdata.blob.core.windows.net/container1' --recursive=true

B aws s3 cp s3://mybucket/test.txt https://consiliumdata.blob.core.windows.net/container1

C azcopy blob copy 'https://s3.amazonaws.com/myS3Bucket' 'https://consiliumdata.blob.core.windows.net/container1'

D azcopy copy sync 'https://s3.amazonaws.com/myS3Bucket' 'https://consiliumdata.blob.core.windows.net/container1'

3\. You create an Azure storage account named consiliumstore with a publicly accessible container named container1\. You upload a file to container1 named pic1\.png\. What will be the URL in order to access this blob?
A https://consiliumstore.blob.core.windows.net/container1/pic1.png

B https://portal.azure.com/consiliumstore.blob.core.windows.net/pic1.png

C https://blob.core.windows.net/consiliumstore/container1/pic.png

D https://pic1.consiliumstore.blob.core.windows.net

4\. You have been directed to copy all data from one storage account to another using the AzCopy tool\. You need to report which storage services you can copy\. Which of those services would it be?

A Only Azure File Shares

B Azure Queues and Blobs

C Azure Blob and File Shares

D Azure Table and File Shares

5\. You have an existing Microsoft Enterprise Agreement \(EA\) Subscription\. You need to ship 34TB of data from an on\-premise Windows 2016 server to your Azure storage account\. You need to ensure that the data transfer has zero impact on the network\, preserves your existing drives and is the fastest and most secure method\. What should be your first step to starting the import job?

A Open a ticket with Microsoft Support

B Order an Azure Databox via the Azure Portal

C Start an Import Job via the Azure Portal

D Prepare your hard drives using the WAImportExport tool

6\. Your on\-premise network consists of two servers named Serve1 and Serve2\, both running Windows Server 2019 Datacenter\. On Serve1\, a file exists named file1\.txt\. On Serve2\, a file exists also named file1\.txt\, but its contents are different\. You set up a file sync service in Azure to sync the folders that contain both versions of file1\.txt to a cloud endpoint\. First\, you setup Serve1 as a server endpoint\, then a few hours later\, Serve2\. What will happen to file1\.txt?

A file1.txt on Serve1 will be renamed file1-old.txt

B file1.txt will be overwritten as soon as Serve2 server endpoint is added

C file1.txt on Serve1 will be moved to another folder

D file1.txt from Serve1 is renamed file1-Serve1.txt

7\. You have a general purpose v1 storage account named consiliumstore that has a private container named container2\. You need to allow read access to the data inside container2\, but only within a 14 day window\. How do you accomplish this using the Azure Portal?

A Upgrade the storage account to general purpose v2

B Create a shared access signatures

C Create a service SAS

D Create a stored access policy

Answers: (1) D (2) A (3) A (4) C (5) B (6) D (7) B, D