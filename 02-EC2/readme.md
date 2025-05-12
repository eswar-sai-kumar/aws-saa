# 02-EC2

We can SSH into your EC2 instance using tools like putty, mobaxterm etc

Also we can do it by EC2 instance connect

Create instance → connect

![Screenshot 2025-05-10 194239](https://github.com/user-attachments/assets/721f5649-d574-473e-80af-df1eee74c321)\

connect using ec2 instance connect → connect

![Screenshot 2025-05-10 194255](https://github.com/user-attachments/assets/2316c7f8-7901-458b-bf80-d7abb25cd5d8)

![Screenshot 2025-05-10 194443](https://github.com/user-attachments/assets/3bc5be13-657d-44f5-bafc-362615843262)



### IPAM

IPAM stands for IP Address Manager in AWS.

🌐 What is IPAM?
AWS IPAM helps you organize, track, assign, and manage IP addresses (both IPv4 and IPv6) across all your AWS accounts and regions.

🔧 Why use IPAM?
Without IPAM:

You manually track IPs (e.g., in spreadsheets 😩).

You risk IP conflicts or wasted IPs.

###### With IPAM:

AWS automatically manages IPs.

Helps you allocate, monitor, and audit IP addresses.

Supports VPC creation, subnet management, and multi-account IP sharing.

IPAM → Amazon VPC IP adddress manager 

![image](https://github.com/user-attachments/assets/999c9817-1e34-4d97-911f-dcca092912d5)

Create IPAM → ✅ allow amazon VPC IP → Free tier

![image](https://github.com/user-attachments/assets/562eebed-2a9c-4736-922f-fb5ba571b3af)

Operating regions(add all regions) 

![image](https://github.com/user-attachments/assets/29e88fae-b8c6-4add-a7c2-6891ba56b570)

create

![image](https://github.com/user-attachments/assets/cb9dd0cd-d008-4fb8-a767-8db2dd960fa6)

public IP insights → 

![image](https://github.com/user-attachments/assets/c0882baa-7276-4573-874e-76f37d093f8b)

### Elastic IP

If we stop instance and start instance, public IP changes. 

So we use Elastic IP. Elastic IP wont change public IP

### Creating Elastic IP

EC2 → Elastic IP Address → Amazon pool of IPV4 → allocate → actions → associate elastic IP → click instance → Instance → private IP → allocate

### Placement groups

🔶 What is a Placement Group?

A Placement Group in AWS helps you control how EC2 instances are placed on underlying hardware to meet specific performance or fault tolerance needs.

1. Cluster Placement Group
   
✅ Purpose: High performance

📍 Placement: Instances are placed close together (in the same rack or host).

⚡ Best for: Applications needing low latency and high throughput (like HPC, big data).

❗ Downside: If the rack fails, all instances may be affected.

2. Spread Placement Group
   
✅ Purpose: High availability

📍 Placement: Instances are placed far apart (different racks or hardware).

🛡️ Best for: Critical applications that must avoid single point of failure.

📦 Limit: Max 7 instances per AZ per group.

3. Partition Placement Group
   
✅ Purpose: Balance between performance and fault tolerance

📍 Placement: Instances are divided into partitions (each partition in separate hardware).

🧠 Best for: Large-scale distributed systems (e.g., Hadoop, Cassandra).

🔁 Fault isolation: Failure in one partition doesn’t affect others.



### Creating placement groups

Instances → Placement groups → Name → Choose(Cluster, spread or partition) → Craete group

EC2 → Launch EC2 instance → adv details → Placement group name → can select group

### Elastic network interface (ENI)






