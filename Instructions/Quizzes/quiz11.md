## Quiz 11
<br>
1\\. You have a number of virtual machines and web applications running in your Azure environment. These Azure resources are critical for business operations, so you've locked the resources in order to prevent deletion. In addition, how can you alert on these actions in the portal, and notify your team via email and SMS when a user is trying to delete or create a new resource from within your Azure subscription?
A  Pin the activity log to your dashboard

B  Create a new alert rule

C  Query Administrative Events and Copy Link to Query

D  Create a new action group

<br>
2\\. You have an Azure subscription named Subscription1. In Subscription1 you have two Azure VMs named VM1 and VM2, both running Windows Server 2016. VM1 is backed up using Recovery Services Vault, with a backup policy of producing a daily backup and keeping that daily backup for seven days. Also, a snapshot is kept for 2 days. VM1 is compromised by a virus that infects the entire system, including the files. You need to restore the files from yesterday's backup of VM1. Where can you restore the files to in the quickest manner?
A  A new Azure VM

B  Restore the VM1 snapshot

C  VM2

D  In-place

3\\. You have a subscription named Subscription1. You would like to be alerted upon certain administrative events within Subscription1 to detect unauthorized access. Which of the following is the quickest method to setup these types of alerts?

A  Monitor > Alerts > New Alert Rule

B  Log Analytics Workspace > myWorkdspace > Advanced Settings

C  Policy > Assignments > Assign Policy

D  Subscriptions > mySubscription > Activity Log > New Alert

4\\. You have an Azure subscription with a virtual machine named VM1. You are using Recovery Services Vault (RSV) to backup VM1 with soft delete enabled. The backup policy is set to backup daily at 11 PM UTC, retain an instant recovery snapshot for 2 days, and retain the daily backup point for 14 days. After the initial backup of VM1, you are instructed to delete the vault and all of the backup data. What should you do?

A  Turn off soft delete in the vault security settings

B  Wait 14 days

C  Stop the backup of VM1 and delete backup data

D  Delete the backup policy

E  Delete Backup Jobs Workload

F  Wait 15 days

5\\. You have an Azure subscription named Subscription1. In Subscription1, you have an Azure virtual machine named VM1. In order to create a daily backup of VM1, starting at 11:00 PM and retaining a copy of the backup for recovery purposes for seven days, what are the two items I will need in order to store the backup and configure the schedule?

A  A Recovery Services Vault

B  A Backup Policy

C  A Batch File

D  A Cron Job

<br>
6\\. You have a .NET Core application running in Azure App Services. You are expecting a huge influx of traffic to your application in the coming days. When your application experiences this spike in traffic, you want to detect any anomalies such as request errors or failed queries immediately. What service can you use to assure that you know about these types of errors related to your .NET application immediately?

A  Client-side monitoring

B  Live Metrics Stream in Application Insights

C  Application Insights Search

D  Log analytics workspace

<br>
7\\. You have an Azure virtual machine running Windows Server 2016. You need to collect OS level metrics on this virtual machine, including Windows event logs and performance counters. Which of the following items do you need in order to collect this metrics data?

A  Enable guest-level monitoring

B  Windows Diagnostics Extension

C  Log Analytics Agent

D  InfluxData Telegraf Agent

E  Storage Account for Diagnostic Data

Answers: (1) B, D (2) B (3) A (4) A, C (5) A, B (6)  B (7) A, B, C