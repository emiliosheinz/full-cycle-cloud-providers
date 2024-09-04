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

