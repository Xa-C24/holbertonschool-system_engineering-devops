Web Infrastructure Design

This repository contains the design and explanation of various web infrastructure setups, detailing their components, roles, and issues, as part of the Holberton School System Engineering and DevOps track.

Concepts Covered

The project explores the following concepts:

Network Basics

Server Basics

Web Server and Application Server

Domain Name System (DNS)

Load Balancer

Monitoring

Database Management

Learning Objectives

By completing this project, you should be able to:

Draw and explain the web stack you designed.

Describe the role of each component in your infrastructure.

Understand system redundancy and high availability.

Explain relevant acronyms such as LAMP, SPOF, and QPS.

Tasks

Task 0: Simple Web Stack

Description

Design a one-server web infrastructure to host a website accessible via www.foobar.com.

Components

1 Server (IP: 8.8.8.8)

1 Web Server (Nginx)

1 Application Server

1 Database (MySQL)

1 Domain Name with www DNS record

Requirements

Explain the role of:

Server

Domain Name

Web Server

Application Server

Database

Address potential issues:

Single Point of Failure (SPOF)

Downtime during maintenance

Scalability limitations

Deliverables

File: 0-simple_web_stack

Diagram: Upload a screenshot of your whiteboarded design.

Task 1: Distributed Web Infrastructure

Description

Design a three-server web infrastructure to host www.foobar.com, adding redundancy and distribution.

Components

2 Servers for web and application

1 Load Balancer (HAproxy)

1 MySQL Database

Requirements

Explain the purpose of:

Load Balancer

Distribution algorithms

Active-Active vs. Active-Passive setup

Database Primary-Replica cluster

Address potential issues:

Remaining SPOF

Lack of security measures

No monitoring

Deliverables

File: 1-distributed_web_infrastructure

Diagram: Upload a screenshot of your whiteboarded design.

Task 2: Secured and Monitored Web Infrastructure

Description

Enhance the three-server infrastructure with security and monitoring features.

Components

3 Firewalls

1 SSL Certificate (HTTPS)

3 Monitoring Clients (e.g., Sumologic)

Requirements

Explain the purpose of:

Firewalls

HTTPS encryption

Monitoring tools

Monitoring QPS for the web server

Discuss issues:

SSL termination at the load balancer

Single MySQL server writes

Component homogeneity risks

Deliverables

File: 2-secured_and_monitored_web_infrastructure

Diagram: Upload a screenshot of your whiteboarded design.

Task 3: Scale Up

Description

Scale the web infrastructure by adding redundancy and splitting components across multiple servers.

Components

1 Additional Server

1 Load Balancer Cluster (HAproxy)

Split:

Web Server

Application Server

Database

Requirements

Explain:

Why each component was added

Impact on system performance and availability

Deliverables

File: 3-scale_up

Diagram: Upload a screenshot of your whiteboarded design.

Repository Structure

holbertonschool-system_engineering-devops/
|-- web_infrastructure_design/
    |-- 0-simple_web_stack
    |-- 1-distributed_web_infrastructure
    |-- 2-secured_and_monitored_web_infrastructure
    |-- 3-scale_up

How to Use

Clone this repository:

git clone https://github.com/your_username/holbertonschool-system_engineering-devops.git

Navigate to the project directory:

cd web_infrastructure_design

Review each task file and corresponding diagrams.