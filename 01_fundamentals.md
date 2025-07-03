# AWS Fundamentals

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

## Security, Identity & Compliance

- **IAM (Identity and Access Management)**: user management and access level to AWS resources.
- **Cognition**: Device authentication, OAuth service. Provides temporary access to AWS resources.
- **Guard duty**: Monitor for malicious activity.
- **Inspector**: Agent install in VMs you can test security vulnerabilities.
- **Macie**:Check for personally identifiable information. Alerts and gives visibility on how PII data is accessed or moved.
- **Certificate Manager**: It is used to give certificates to any domain you have registered via AWS/Routes 53. This also helps in maintaining and updating certificates that are about to expire.
- **Cloud HSMHardware Security Module**: It is a dedicated hardware to store your hardware private and public keys, that are used to securely access your application/EC2 instances. You can also store a variety of exception keys.
- **Directory Services**: It is used for integrating your Microsoft active directory services with AWS services.
- **WAF – Web Application Firewall**: WAF sits in front of your web server and it mitigates against injection, cross-scripting. WAF primarily protects your application layer from any malicious attacks
- **Shield**: You get this as a default for your load balancers, cloud front, as well as Route 53. This is basically a DDoS mitigation service that prevents DDoS Attacks.
- **Advance Shield**: It is an AWS team that is in standby mode in the case of a DDOS attack. If you have advanced shield protection, then AWS will not charge you for any auto-scaling or added utilization of the AWS services during the attack.
- **Artifact**: It is used for compliance and audit. Artifact gives access to AWS SOC 1, 2, 3, PCI reports, etc. It is a central resource for compliance-related information that matters to you. It provides on-demand access to AWS’ security posture.
