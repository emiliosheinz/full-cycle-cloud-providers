# Cloud Providers


Cloud computing is a technology that allows users to access and store data, run applications, and perform various computing tasks over the internet rather than on local servers or personal computers. It provides on-demand access to a shared pool of configurable computing resources, such as servers, storage, databases, and software, which can be rapidly provisioned and released with minimal management effort. This model offers scalability, flexibility, cost efficiency, and the ability to access services from anywhere with an internet connection.

![Types of computing service](./docs/images/types-of-service.png)

## Amazon Web Services (AWS)

AWS was created in 2006 and is currently the world's most comprehensive and broadly adopted cloud platform, offering over 200 fully featured services from data centers globally. Millions of customers, including the fastest-growing startups, largest enterprises, and leading government agencies, trust AWS to power their infrastructure, become more agile, and lower costs.

### Regions and Availability Zones

AWS has the most extensive global cloud infrastructure, with 77 Availability Zones within 24 geographic regions around the world, with plans for 18 more Availability Zones and six more AWS Regions in Australia, India, Indonesia, Spain, Switzerland, and the United Arab Emirates.

- **Region**: A region is a physical location in the world where AWS has multiple Availability Zones. Each region is a separate geographic area, and each region has multiple, isolated locations known as Availability Zones.

- **Availability Zone**: An Availability Zone is one or more discrete data centers with redundant power, networking, and connectivity in the same region. Availability Zones are isolated from each other to prevent failures from spreading between Zones.

For more information about Regions and Availability Zones, visit the [official website](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/).

### Local Zones

AWS Local Zones are a type of infrastructure deployment that places select AWS services closer to your end users and workloads. They are ideal for use cases such as real-time gaming, hybrid migrations, and media & entertainment content creation that require single-digit millisecond latency for end-users in specific geographic areas. Unfortunatelly, Local Zones are not available in all regions and not all services are available in Local Zones.

### Wavelength Zones

AWS Wavelength brings AWS services to the edge of the 5G network, minimizing the latency to connect to an application from a mobile device. This allows developers to build applications that deliver single-digit millisecond latencies to mobile devices and end-users.

### Identity and Access Management (IAM)

AWS Identity and Access Management (IAM) enables you to manage access to AWS services and resources securely. Using IAM, you can create and manage AWS users and groups, and use permissions to allow and deny their access to specific AWS resources.

- **User**: A person or service that interacts with AWS resources. 

- **Group**: A collection of users under one set of permissionA set of permissions grouped together that you can apply to a user or group.s.

- **Role**: Permissions that are linked to a specific service or function. Roles are used to delegate access to users, applications, or services that don't normally have access to AWS resources.

- **Policy**: A policy is an object in AWS that, when associated with an identity or resource, defines their permissions. Policies are stored in AWS as JSON documents.

### Elastic Compute Cloud (EC2)

Amazon EC2 is a web service provided by AWS that allows users to rent virtual servers, known as instances, to run applications on the cloud. EC2 offers scalable computing capacity, enabling users to easily scale up or down based on demand. It provides a variety of instance types optimized for different workloads, such as computing, memory, or storage-intensive tasks. EC2 also supports multiple operating systems and integrates with other AWS services, making it a flexible and powerful solution for deploying and managing applications in the cloud.

### Virtual Private Cloud (VPC)

Amazon Virtual Private Cloud (VPC) is a service that allows users to create a private, isolated section of the AWS cloud where they can launch resources, such as EC2 instances, within a virtual network. VPC provides control over the network configuration, including IP address ranges, subnets, route tables, and network gateways. Users can also create security groups and network access control lists to control inbound and outbound traffic to their instances. In other words, VPC enables users to build a secure and scalable environment in the cloud.

#### Subnets

A subnet is a range of IP addresses withing a VPC, used to segment and isolate network resources withi a cloud environment. Subnets can be public, private, or dedicated to a specific resource. A public subnet typically allows internet access via a route through an Internet Gateway (IGW), while a private subnet does not, restricting access to internal resources only. 

#### Internet Gateway (IGW)

An Internet Gateway (IGW) is a horizontally scaled, redundant, and highly available VPC component that allows communication between instances in a VPC and the internet. It provides a target in your VPC route tables for internet-routable traffic, and it performs network address translation (NAT) for instances that have been assigned public IPv4 addresses.

#### Route Tables

A route table contains a set of rules, called routes, that are used to determine where network traffic is directed. Each subnet in a VPC must be associated with a route table, which controls the routing for the subnet. The route table specifies how packets are forwarded between the subnet and the gateway, such as an Internet Gateway (IGW) or a Virtual Private Gateway (VGW).

#### Bastion Host

A Bastion Host is a hardened instance used to securely access resources in private subnets. It acts as a gateway, typically allowing SSH or RDP access while minimizing attack surfaces by restricting unnecessary services and limiting external exposure.

#### NAT Gateway

A NAT gateway is a managed network address translation (NAT) service that enables instances in a private subnet to connect to the internet or other AWS services, but prevents the internet from initiating a connection with those instances. It allows instances in a private subnet to access the internet while remaining private and secure.

#### Security Groups

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. When you launch an instance in a VPC, you can assign up to five security groups to the instance. Security groups act at the instance level, not the subnet level. Therefore, each instance in a subnet in your VPC can be assigned to a different set of security groups.
