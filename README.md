# refactor-aws-multi-tier-webapp
Rearchitect multi tier web application from VMs to AWS Cloud Native application

Project 03 DevOps

The Multi Tier web Application from Project 01 is refactored to a cloud native application in AWS.
AWS Beanstalk is used to run the web applicaiton server (Tomcat).
RDS Instance is used for databases instead of MySQL.
Elasti cache is used instead of memcache.
Active MQ replaces Rabbit MQ.
Route 53 is used for the DNS.
CloudFront for the Contend Delivery Network.

Since RDS is in private VPC, create EC2 instance in same VPC to access RDS and run queries.
