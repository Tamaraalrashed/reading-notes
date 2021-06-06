# AWS: Cloud Servers

## Review, Research, and Discussion

### Describe the Web-Request-Response-Cycle

1. A user opens his browser, types in a URL, and presses Enter.
1. When a user presses Enter, the browser makes a request for that URL.
1. The request hits the Rails router (config/routes.rb). The router maps the URL to the correct controller and action to handle the request.
1. The action receives the request and passes it on to the view.
1. The view renders the page as HTML.
1. The controller sends the HTML back to the browser. The page loads and the user sees it. <br>

### Explain what a “server” is, as it relates to the WRRC

The Server(computer)reads the HTTP Request,and generates an HTTP Response to that Request.It hands the Response off to their ISP and it goes through the internet to arrive at the client computer.<br>

### What does it mean to “deploy” an application?

 It refers to the process of running an application on a server or device.<br>


## Terms

### Server

 A computer that serves information to other computers.<br>

### Pub/Sub

Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic.<br>

### WRRC

Web Request Response Cycle server.<br>

## Preparation Materials


### - Virtual Machines

Virtual Machine (VM) is a compute resource that uses software instead of a physical computer to run programs and deploy apps.<br>

Virtual machines (VMs) allow a business to run an operating system that behaves like a completely separate computer in an app window on a desktop. VMs may be deployed to accommodate different levels of processing power needs, to run software that requires a different operating system, or to test applications in a safe, sandboxed environment. <br>

The two types of virtual machines 
Users can choose from two different types of virtual machines—process VMs and system VMs:  <br>

A process virtual machine allows a single process to run as an application on a host machine, providing a platform-independent programming environment by masking the information of the underlying hardware or operating system. An example of a process VM is the Java Virtual Machine, which enables any operating system to run Java applications as if they were native to that system.   <br>

A system virtual machine is fully virtualized to substitute for a physical machine. A system platform supports the sharing of a host computer’s physical resources between multiple virtual machines, each running its own copy of the operating system. This virtualization process relies on a hypervisor, which can run on bare hardware, such as VMware ESXi, or on top of an operating system. <br>

### Amazon Elastic Compute Cloud

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.

Amazon EC2 offers the broadest and deepest compute platform with choice of processor, storage, networking, operating system, and purchase model. We offer the fastest processors in the cloud and we are the only cloud with 400 Gbps ethernet networking. We have the most powerful GPU instances for machine learning training and graphics workloads, as well as the lowest cost-per-inference instances in the cloud. More SAP, HPC, Machine Learning, and Windows workloads run on AWS than any other cloud. Click here to learn What's New with Amazon EC2.

### AWS Elastic Beanstalk

AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS.<br>

You can simply upload your code and Elastic Beanstalk automatically handles the deployment, from capacity provisioning, load balancing, auto-scaling to application health monitoring. At the same time, you retain full control over the AWS resources powering your application and can access the underlying resources at any time.<br>

There is no additional charge for Elastic Beanstalk - you pay only for the AWS resources needed to store and run your applications.<br>




