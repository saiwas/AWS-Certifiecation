# AWS Cloud Practitioner Essentials

## AWS Cloud Interface

1. Three way to use AWS:
    + AWS Management Console
      > Easy to use graphical interface that supports majority of AWS.
    + AWS Command Line Interface(CLI)
      > Access to services via discrete command.
    + Software Development Kits(SDKs)
      > Incorporate the connectivity and functionality of the wide range of AWS Cloud services into your code.

1. Create your own resource
1. Access features on the go

## AWS Core Services

  1. Elastic Cloud Computer(EC2)
      + Product Demonstration
          1. Login to the AWS Console.
          1. Choose a region
          1. Launch EC2 Wizard
          1. Select AMI(SW) - Amazon Machine Image
          1. Select instance type
          1. Configure Network
          1. Configure Storage
          1. Configure Key pair
          1. Launch & connect
  1. Elastic Block Store(EBS)
  1. Amazon Simple Storage Service(S3)
      + Introduction
          1. Managed cloud storage service
          1. Store virtual unlimited number of objects
          1. Access any time from anywhere
          1. Rich security controls

      + Common Cases
          1. Storing Application Asserts
          1. Statics Web Hosting
          1. Backup & Disaster Recovery
          1. Staging area for Big Data

  1. AWS Global Infrastructure
      1. Region
      1. Availability Zone
      1. Edge Locations

  1. Amazon Virtual Private Cloud(VPC)
      + Introduction
        1. A private, virtual network in AWS cloud
            > Uses same concepts as on the premise network
        1. Allows complete control of network configuration
            > Ability to isolate and expose resources inside VPC
        1. Offers several layers of security controls
            > Ability to allow and deny specify internet and internal traffic
        1. Other AWS deploy to VPC
            > Service inherent security built into network

      + Features
        1. Build upon high availability of AWS Regions and Availability Zone(AZ)
            > Amazon VPC lives within Region, Multiple VPC per account
        1. Subnets
            > Use to divide amazon VPC, Allow amazon VPC to span multiple AZs
        1. Route tables
            > Control traffic going out of the subnets
        1. Internet Gateway (IGW)
            > Allow access to the internet from Amazon VPC
        1. NAT Gateway
            > Allows private subnet resources to access internet
        1. Network Access Control Lists (NACL)
            > Control access to subnets, stateless
  1. Security Groups
      1. Act as built-in firewalls
      1. Control accessibility to the instance
