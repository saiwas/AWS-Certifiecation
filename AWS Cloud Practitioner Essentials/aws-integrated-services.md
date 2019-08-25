# AWS Integrated Services

  1. Application Load Balancer
      + Type
         + Classic Load Balancer
         + Network Load Balancer
      + Enhanced Features
        + Supported Protocols
          > HTTP, HTTPS, HTTP/2 and WebSockets
        + CloudWatch Metrics
          > Additional load balance metrics and Target Group metrics dimension
        + Access Logs
          > Ability to see connection detail for WebSocket connects
        + Health Checks
          > Insight into target and application health at more granular level
      + Additional Features
        + Path and Host-based Routing
          > Path-based provides rules that forward requests to different target groups (Added Feature)

          > Host-based can be used to define rules that forward requests to different target groups based on host name(Added Feature)
        + Native IPv6 Support
        + AWS WAF(Web Application Firewall)
        + Dynamic Ports
          > Amazon ECS integrates with Application Load Balancer to expose Dynamic Ports utilized by scheduled containers.
        + Deletion Protection & Request Tracing
          > Request tracing can be used to track HTTP requests from clients to target(Added Feature)
      + Key Terms
        + Listeners
          > A listener is process that checks for connection requests, using the protocol and port that you configure. The rules that you define for a listener determine how the load balancer routes requests to the targets in one or more target groups.
        + Target
          > A target is a destination for the traffic based on the established listener rules.
        + Target Group
          > Each target group routes requests to one or more registered targets using the protocol and port number specified. A target can be registered with multiple target groups. Health checks can be configured on a per target group basic.
      + Use Cases
        1. To host the micro services and route to the application in a single load balancer
          ![load-balancer](./asserts/load-balancer-1.png)
          ![load-balancer](./asserts/load-balancer-2.png)

  1. Auto Scaling
      > Auto Scaling helps you ensure that you have the correct number of Amazon EC2 instances available to handle the load for your application ![load-balancer](./asserts/auto-scaling-1.png)

      + Auto Scaling Components
        1. Launch Configuration (What to be run)
            + AMI
            + Instance type
            + Security Groups
            + Roles
        1. Auto Scaling Group(Where to be run)
            + VPC and Subnet(s)
            + Load balancer
            + Minimum instances
            + Maximum instances
            + Desired capacity
        1. Auto Scaling Policy(When to be run)
            + Scheduled
            + On-demand
            + Scale-out policy
            + Scale-in policy
      + Dynamic Auto Scaling
        ![load-balancer](./asserts/auto-scaling-2.png)

  1. Amazon Route 53
  1. Amazon Relation Database Services(RDS)
  1. AWS lambda
  1. AWS Elastic Beanstalk
  1. Amazon Simple Notification Service(SNS)
  1. Amazon CloudWatch
  1. Amazon CloudFront
  1. AWS CloudFormation
