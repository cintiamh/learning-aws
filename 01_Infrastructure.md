## Amazon web services infrastructure

### Compute

- **Compute (EC2)**: VMs (OS, RAM, CPU)
- **Elastic Container Services (ECS)**: Docker, "managed" Kubernetes
- **LightSail (VPS Service - Virtual Private Service)**: Virtual private servers, VMs with individual operating systems but restricted access to physical server resources.
- **Lambda**: functions. Pay by function execution.
- **Batch**: batch processing. Dynamic provision compute resources for the given batch process.

### Storage

- **Simple Storage Service (S3)**: object storage service. Data lakes, cloud-native applications, mobile apps.
- **Network Attached Storage (EFS)**: upload files to a EFS and then mount into multiple VMs.
- **Glacier**: Data archival. Lower cost. 3 - 5 hours to restore - $0.01 per gigabyte per month.
- **Snow Ball**: transport large amount of data in or out of AWS (hardware).
- **Storage Gateway**: VM you install in your data center and this replicates data back into S3.

### Database

- **Relational Database Service (RDS)**: Cost-efficient and resizable capacity. Manages database administration tasks (DB sofware patches, backups, recovery). (Amazon Aurora, MySQL, PostgreeSQL, MariaDB, Oracle, and SQL Server)
- **Aurora**: AWS Relational DB compatible with MySQL and PostgreSQL.
- **DynamoDB**: Non relational DB, managed by AWS.
- **Neptune**: Fully managed graph DB. Graph databases use nodes to store data entities, and edges to store relationships between entities.
- **ElasticCache**: fully managed Redis and Memcached.

### Network

- **CloudFront**
- **VPC**
- **Direct Connect**
- **Load Balancing**
- **Route 53**
