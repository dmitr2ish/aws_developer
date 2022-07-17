# aws_developer

####  Describing of aws services
  - ****Compute****
    - **Amazon EC2**.   
      EC2 is Amazon's service that allows you to create a server (AWS calls these instances) in the AWS cloud. You pay by the hour and only what you use. You can do whatever you want with this instance as well as launch n number of instances.
    - **AWS Elastic Beanstalk**.  
    Elastic Beanstalk is one layer of abstraction away from the EC2 layer. Elastic Beanstalk will setup an "environment" for you that can contain a number of EC2 instances, an optional database, as well as a few other AWS components such as a Elastic Load Balancer, Auto-Scaling Group, Security Group. Then Elastic Beanstalk will manage these items for you whenever you want to update your software running in AWS. Elastic Beanstalk doesn't add any cost on top of these resources that it creates for you. If you have 10 hours of EC2 usage, then all you pay is 10 compute hours.
  - ****Containers****
    - **Amazon ECS**.  
    is the AWS solution for managing containers at scale. It helps you speed up the process of building, deploying and migrating your containerized applications. Designed with simplicity in mind, Amazon ECS reduces the burden of setting up network, compute and security configurations, and managing scalability. For example, you don’t need to build a generalized abstraction if you need a load balancer—ECS seamlessly integrates features such as AWS Application Load Balancer (ALB) and Network Load Balancer (NLB).
    - **Amazon EKS**.  
    can handle the heavy lifting of building and running Kubernetes workloads at scale. Kubernetes is known for its vibrant community and ecosystem, open-source APIs and broad flexibility. With EKS, you can access the full power of Kubernetes features, while enjoying the convenience of a managed cloud service.
  - ****Servless****
    - **AWS Lambda**.   
    AWS Lambda is a serverless compute service that runs your code in response to events and automatically manages the underlying compute resources for you. These events may include changes in state or an update, such as a user placing an item in a shopping cart on an ecommerce website.
    - **WS Fargate**.   
    AWS Fargate is a serverless, pay-as-you-go compute engine that lets you focus on building applications without managing servers. AWS Fargate is compatible with both Amazon Elastic Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS).  
    
    While Fargate is a Container as a Service (CaaS) offering, AWS Lambda is a Function as a Service (FaaS offering). Therefore, Lambda functions do not necessarily need to be packaged into containers, making it easier to get started with Lambda. But if you have containerized applications, Fargate is the way to go.
  - ****Storage****
    - **Amazon S3**.  
    Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.
  - ****Relational****
    - **Amazon RDS**.  
    Amazon Relational Database Service (RDS) is a managed SQL database service provided by Amazon Web Services (AWS). Amazon RDS supports an array of database engines to store and organize data. It also helps with relational database management tasks, such as data migration, backup, recovery and patching.
    - **Amazon Aurora**.  
    Amazon Aurora is a relational database management system (RDBMS) built for the cloud with full MySQL and PostgreSQL compatibility. Aurora gives you the performance and availability of commercial-grade databases at one-tenth the cost.
    
    Amazon Aurora is an affordable cloud based relational database compatible with MySQL and PostgreSQL. As a part of Amazon RDS, management of an Aurora database is automated. Data is automatically backed up to Amazon S3 (Simple Storage Service). Multiple instances of the data is maintained for availability and failovers.
    Unlike Amazon RDS for PostgreSQL, where high write workloads can severely impact replication, Aurora uses shared storage for writer and readers. As a result, all Aurora replicas are synced with the writer instance with minimal replica lag. The lag can be different for different replicas
  - ****Non-relational****
    - **Amazon DynamoDB**.  
    Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-Region replication, in-memory caching, and data export tools.
  - ****Identity services****
    - **AWS Identity and Access Management**.  
    AWS Identity and Access Management (IAM) provides fine-grained access control across all of AWS. With IAM, you can specify who can access which services and resources, and under which conditions. With IAM policies, you manage permissions to your workforce and systems to ensure least-privilege permissions.
    - **Amazon Cognito**.  
    Amazon Cognito lets you easily add user sign-up and authentication to your mobile and web apps. Amazon Cognito also enables you to authenticate users through an external identity provider and provides temporary security credentials to access your app's backend resources in AWS or any service behind Amazon API Gateway.
    - **AWS Directory Service**.   
    AWS Directory Service provides multiple directory choices for customers who want to use existing Microsoft AD or Lightweight Directory Access Protocol (LDAP)–aware applications in the cloud. It also offers those same choices to developers who need a directory to manage users, groups, devices, and access.
  - ****Monitoring and auditing services****
    - **Amazon CloudWatch**.  
    Amazon CloudWatch is a monitoring and management service that provides data and actionable insights for AWS, hybrid, and on-premises applications and infrastructure resources.
    - **AWS CloudTrail**.  
    AWS CloudTrail is an AWS service that helps you enable governance, compliance, and operational and risk auditing of your AWS account. Actions taken by a user, role, or an AWS service are recorded as events in CloudTrail.


#### 1.    AWS Elastic Beanstalk - service for quickly deploy app to cloud
    1.1. create app
    1.2. choose server environment
    1.3. choose platform and upload code
    1.4. choose harware configure
    1.5. wait deploy
    1.6. after that your app will avaibale by link on dashboard
    
#### 2.     Getting Started with .NET on AWS
    1.1. choose your version of .net
      1.1.1. for windows .net framework
      1.1.2. for linux, macos and windows .net core - supports moving to the upcoming releases of .net5 and .net6
