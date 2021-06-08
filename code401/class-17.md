# AWS: Cloud Servers

## Review, Research, and Discussion

### Describe “The Cloud”

"The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines. <br>

### What is a container (as it relates to computers and servers)?

 A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. 
 Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure.<br>


### What is auto-scaling?

AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it’s easy to setup application scaling for multiple resources across multiple services in minutes.

### What is bandwidth?

The maximum amount of data transmitted over an internet connection in a given amount of time. <br>

### How do cloud providers compute service costs?

When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.<br>


## Terms

### Server Instances 

A server instance is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.<br>

### Containers

are an executable unit of software in which application code is packaged, along with its libraries and dependencies, in common ways so that it can be run anywhere, whether it be on desktop, traditional IT, or the cloud.<br>

### Cloud Services

Infrastructure, platforms, or software that are hosted by third-party providers and made available to users through the internet. <br>

### Cloud Architecture

It refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems..<br>

### AWS

Amazon Web Services (AWS) is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis.<br>

### EC2/Beanstalk vs Heroku

AWS Elastic Beanstalk and Heroku can be categorized as "Platform as a Service" tools.

Some of the features offered by AWS Elastic Beanstalk are:

Elastic Beanstalk is built using familiar software stacks such as the Apache HTTP Server for Node.js, PHP and Python, Passenger for Ruby, IIS 7.5 for .NET, and Apache Tomcat for Java
There is no additional charge for Elastic Beanstalk - you pay only for the AWS resources needed to store and run your applications.
Easy to begin – Elastic Beanstalk is a quick and simple way to deploy your application to AWS. You simply use the AWS Management Console, Git deployment, or an integrated development environment (IDE) such as Eclipse or Visual Studio to upload your application
On the other hand, Heroku provides the following key features:

Agile deployment for Ruby, Node.js, Clojure, Java, Python, Go and Scala.
Run and scale any type of app.
Total visibility across your entire app. .<br>

## Preparation Materials


### - Amazon S3

Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.

### - AWS Lambda

AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.<br>

The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services. <br>

Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete. <br>

### - Content Delivery Network (CDN)

A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.<br>

CDNs are something that larger companies are more likely to implement. The main reasons why company want to use CDNs are to improve Internet website load speeds, content delivery speeds, and to reduce the likelihood of falling victim to and improve defenses against Distributed Denial of Service attacks (DDoS).<br>





