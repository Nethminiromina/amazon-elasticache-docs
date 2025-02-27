# Amazon ElastiCache ElastiCache for Memcached User Guide

-----
*****Copyright &copy;  Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is Amazon ElastiCache for Memcached?](WhatIs.md)
   + [Common ElastiCache Use Cases and How ElastiCache Can Help](elasticache-use-cases.md)
   + [ElastiCache for Memcached resources](WhatIs.FirstTimeUser.md)
   + [ElastiCache for Memcached components and features](WhatIs.Components.md)
   + [Tools for managing your implementation](WhatIs.Managing.md)
+ [Comparing Memcached and Redis](SelectEngine.md)
+ [Getting started with Amazon ElastiCache for Memcached](GettingStarted.md)
   + [Setting up](set-up.md)
   + [Create and connect to a Memcached cluster](deploy-cluster.md)
      + [Step 1: Determine your cluster's requirements](getting-started-determine-requirements.md)
      + [Step 2: Create a cluster](GettingStarted.CreateCluster.md)
      + [Step 3: Authorize access to the cluster](GettingStarted.AuthorizeAccess.md)
      + [Step 4: Connect to the cluster's node](GettingStarted.ConnectToCacheNode.md)
      + [Step 5: Delete your cluster (avoid unnecessary charges)](GettingStarted.DeleteCacheCluster.md)
   + [ElastiCache tutorials and videos](Tutorials.md)
   + [Where do I go from here?](GettingStarted.WhereGoFromHere.md)
+ [Choosing regions and availability zones](RegionsAndAZs.md)
   + [Using local zones with ElastiCache](Local_zones.md)
   + [Using Outposts](ElastiCache-Outposts.md)
+ [Managing nodes](CacheNodes.md)
   + [Connecting to nodes](nodes-connecting.md)
   + [Supported node types](CacheNodes.SupportedTypes.md)
   + [Replacing nodes](CacheNodes.NodeReplacement.md)
   + [ElastiCache reserved nodes](CacheNodes.Reserved.md)
+ [Managing clusters](Clusters.md)
   + [Preparing a cluster](Clusters.Prepare.md)
      + [Determining your requirements](cluster-create-determine-requirements.md)
      + [Choosing your node size](nodes-select-size.md)
   + [Creating a Memcached cluster](Clusters.Create.CON.Memcached.md)
   + [Creating a cluster](Clusters.Create.md)
   + [Viewing a cluster's details](Clusters.ViewDetails.md)
   + [Modifying an ElastiCache cluster](Clusters.Modify.md)
   + [Rebooting a cluster](Clusters.Rebooting.md)
   + [Adding nodes to a cluster](Clusters.AddNode.md)
   + [Removing nodes from a cluster](Clusters.DeleteNode.md)
   + [Canceling pending add or delete node operations](Clusters.CancelPending.md)
   + [Deleting a cluster](Clusters.Delete.md)
   + [Accessing your cluster](accessing-elasticache.md)
   + [Finding connection endpoints](Endpoints.md)
   + [Automatically identify nodes in your cluster](AutoDiscovery.md)
      + [Benefits of Auto Discovery](AutoDiscovery.Benefits.md)
      + [How Auto Discovery Works](AutoDiscovery.HowAutoDiscoveryWorks.md)
      + [Using Auto Discovery](AutoDiscovery.Using.md)
         + [Using the ElastiCache Cluster Client for Java](AutoDiscovery.Using.ModifyApp.Java.md)
         + [Using the ElastiCache Cluster Client for PHP](AutoDiscovery.Using.ModifyApp.PHP.md)
         + [Using the ElastiCache Cluster Client for .NET](AutoDiscovery.Using.ModifyApp.DotNET.md)
      + [Connecting to Cache Nodes Manually](AutoDiscovery.Manual.md)
      + [Adding Auto Discovery To Your Client Library](AutoDiscovery.AddingToYourClientLibrary.md)
      + [ElastiCache clients with auto discovery](Clients.md)
         + [Installing & compiling cluster clients](Appendix.InstallingClients.md)
            + [Installing the ElastiCache cluster client for .NET](Appendix.DotNETAutoDiscoverySetup.md)
            + [Installing the ElastiCache cluster client for PHP](Appendix.PHPAutoDiscoverySetup.md)
               + [Downloading the installation package](Appendix.PHPAutoDiscoverySetup.Downloading.md)
               + [Installation steps for new users](Appendix.PHPAutoDiscoverySetup.Installing.md)
               + [Removing the PHP cluster client](Appendix.PHPAutoDiscoverySetup.Removing.md)
            + [Compiling the source code for the ElastiCache cluster client for PHP](Appendix.PHPAutoDiscoveryCompile.md)
         + [Configuring ElastiCache clients](ClientConfig.md)
            + [Finding node endpoints and port numbers](ClientConfig.FindingEndpointsAndPorts.md)
            + [Connecting for using auto discovery](ClientConfig.AutoDiscovery.md)
            + [DNS names and underlying IP](ClientConfig.DNS.md)
+ [Managing your ElastiCache for Memcached implementation](managing-elasticache.md)
   + [Engine versions and upgrading](engine-versions.md)
      + [Supported ElastiCache for Memcached versions](supported-engine-versions.md)
      + [Upgrading engine versions](VersionManagement.md)
   + [Tagging your ElastiCache resources](Tagging-Resources.md)
      + [Monitoring costs with cost allocation tags](Tagging.md)
      + [Managing your cost allocation tags using the AWS CLI](Tagging.Managing.CLI.md)
      + [Managing your cost allocation tags using the ElastiCache API](Tagging.Managing.API.md)
   + [Caching strategies and best practices](BestPractices.md)
      + [Caching strategies](Strategies.md)
      + [Configuring your ElastiCache client for efficient load balancing](BestPractices.LoadBalancing.md)
   + [Managing maintenance](maintenance-window.md)
   + [Scaling ElastiCache for Memcached clusters](Scaling.md)
   + [Configuring engine parameters using parameter groups](ParameterGroups.md)
      + [Parameter management](ParameterGroups.Management.md)
      + [Cache parameter group tiers](ParameterGroups.Tiers.md)
      + [Creating a parameter group](ParameterGroups.Creating.md)
      + [Listing parameter groups by name](ParameterGroups.ListingGroups.md)
      + [Listing a parameter group's values](ParameterGroups.ListingValues.md)
      + [Modifying a parameter group](ParameterGroups.Modifying.md)
      + [Deleting a parameter group](ParameterGroups.Deleting.md)
      + [Memcached specific parameters](ParameterGroups.Memcached.md)
+ [Security in Amazon ElastiCache](memcached-security.md)
   + [Internetwork traffic privacy](Security.md)
      + [Amazon VPCs and ElastiCache security](VPCs.md)
         + [Understanding ElastiCache and Amazon VPCs](VPCs.EC.md)
         + [Access Patterns for Accessing an ElastiCache Cluster in an Amazon VPC](elasticache-vpc-accessing.md)
         + [Migrating an EC2-Classic cluster into a VPC](Migrating-ec2-classic_to_VPC.md)
         + [Creating a Virtual Private Cloud (VPC)](VPCs.CreatingVPC.md)
         + [Connecting to a cache cluster running in an Amazon VPC](VPCs.Connecting.md)
      + [Subnets and subnet groups](SubnetGroups.md)
         + [Creating a subnet group](SubnetGroups.Creating.md)
         + [Assigning a subnet group to a cluster](SubnetGroups.Assigning.md)
         + [Modifying a subnet group](SubnetGroups.Modifying.md)
         + [Deleting a subnet group](SubnetGroups.Deleting.md)
      + [Security groups: EC2-Classic](SecurityGroups.md)
         + [Creating a security group](SecurityGroups.Creating.md)
         + [Listing available security groups](SecurityGroups.Listing.md)
         + [Authorizing network access to an amazon EC2 security group](SecurityGroups.AuthorizingEC2.md)
   + [Identity and access management in Amazon ElastiCache](IAM.md)
      + [Overview of managing access permissions to your ElastiCache resources](IAM.Overview.md)
         + [Using identity-based policies (IAM policies) for Amazon ElastiCache](IAM.IdentityBasedPolicies.md)
         + [Resource-level permissions](IAM.ResourceLevelPermissions.md)
         + [Using condition keys](IAM.ConditionKeys.md)
         + [Using Service-Linked Roles for Amazon ElastiCache](using-service-linked-roles.md)
         + [ElastiCache API permissions: Actions, resources, and conditions reference](IAM.APIReference.md)
   + [Monitoring usage, events, and costs](MonitoringECMetrics.md)
      + [Monitoring use with CloudWatch metrics](CacheMetrics.md)
         + [Host-Level Metrics](CacheMetrics.HostLevel.md)
         + [Metrics for Memcached](CacheMetrics.Memcached.md)
         + [Which metrics should I monitor?](CacheMetrics.WhichShouldIMonitor.md)
         + [Monitoring CloudWatch Cluster and Node Metrics](CloudWatchMetrics.md)
      + [Logging Amazon ElastiCache API calls with AWS CloudTrail](logging-using-cloudtrail.md)
      + [Monitoring ElastiCache events](ECEvents.md)
         + [Managing ElastiCache Amazon SNS notifications](ECEvents.SNS.md)
         + [Viewing ElastiCache events](ECEvents.Viewing.md)
         + [Event Notifications and Amazon SNS](ElastiCacheSNS.md)
   + [Compliance Validation for Amazon ElastiCache](memcached-compliance.md)
   + [Resilience in Amazon ElastiCache](disaster-recovery-resiliency.md)
      + [Mitigating Failures](FaultTolerance.md)
   + [Infrastructure security in AWS Elasticache](infrastructure-security.md)
   + [Self-service updates in Amazon ElastiCache](Self-Service-Updates.md)
      + [Managing the service updates](managing-updates.md)
         + [Applying the self-service updates](applying-updates.md)
            + [Applying the service updates using the console](applying-updates-console.md)
            + [Applying the service updates using the AWS CLI](applying-updates-cli-memcached.md)
         + [Stopping the self-service updates](stopping-self-service-updates.md)
            + [Stopping the service updates using the console](stopping-updates-console-memcached.md)
            + [Stopping the service updates using the AWS CLI](stopping-updates-cli-memcached.md)
+ [Reference](elasticache-api-reference.md)
   + [Using the ElastiCache API](ProgrammingGuide.md)
      + [Using the query API](ProgrammingGuide.QueryAPI.md)
      + [Available libraries](using-libraries.md)
      + [Troubleshooting applications](Troubleshooting.md)
   + [Amazon ElastiCache error messages](ErrorMessages.md)
   + [Notifications](elasticache-notifications.md)
+ [Documentation history](WhatsNew.md)
+ [AWS glossary](glossary.md)