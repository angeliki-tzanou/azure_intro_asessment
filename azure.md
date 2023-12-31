# Assignment 1: Part 2
# (a & b) Identify & List Services: (Including service description)
## Storage
- **storage accounts:** *to store data in the cloud, gen-purpose storage account to store object data, NoSQL data store, queues for message processing, and file shares in the cloud. Blob storage and hot/cool access tiers are used to optimize costs based on the data accessing frequency of your object data.*
- **storage browser:** *allows to quickly view all the storage services under your account, read, edit, and browse data stored in those services, and manage your cloud storage accounts in multiple subscriptions across all Azure platforms*
- **storage movers:** *a managed migration service that allows you to move on-premises files and folders to Azure storage and minimize downtime for your workload*
- **storage sync services:** *a peer of the storage account resource and create sync groups that contain file shares across multiple storage accounts*
- **disk pools:** *allows you to create a pool of managed disks that can be shared across multiple virtual machines* 

## Compute
- **computer vision:** *a unified service that offers innovative computer vision capabilities*
- **virtual machines:** *one of several types of on-demand, scalable computing resources for Azure, used for when you need more control over the computing environment*
- **saving plans:** *a flexible pricing model*
- **disk accesses:** *high performance and durable block storage for any purpose or any business purposes*
- **cloud services:** *an example of PaaS (platform as a service) designed to support apps that are scalable, reliable, and inexpensive to operate.*

## Database Services
- **SQL databases:** *support modern cloud applications on an intelligent, managed database service, that includes serverless compute*
- **Managed databases:** *automate tasks such as configuring and managing high availability, disaster recovery, backups, and data replications*
- **Data share invitations:** *allows organizations to securely share data with multiple people and partners*
- **SQL virtual machines:** *allows you to use full versions of the SQL server in the cloud without having to directly manage any on-premises hardware*

# c. Python interaction
- Many of these services can be utilized with Python in order to become more productive and efficient especially when combatting a heavy workload. For instance, having storage accounts can ease access to data from any physical device with the same login utilizing its ability of on-demand access. More specifically when considering the direct Python usage Azure SDK can actually provide Python packages that allow to access the Azure services. When using the Azure storage blobs for example for Python you can mainly interact with the storage account directly, the blob storage container, and blobs within the created client for different types of storage data. When using Azure resources such as cloud services, storage accounts movers, and SQL databases, you can integrate the project from Python with those services. By doing so you can use it on Python built apps in the cloud and connect your applications to data through the Azure services for SQL databases. Those services can also be used to build and deploy projects from Python for data science and machine learning purposes, while also debugging the Python apps that you have already created through the editor services while also being able to connect it to GitHub simplifying the process.
