[TOC]

# BoboSystem

The project uses a microservice architecture that can be deployed to the Kubernetes cluster.

### function(relatively simple)

  - The administrator Admin manages the company and the scheduling 
  - employee Worker manages the personal information

### technology

- React 
- SpringBoot
- MySQL
- Docker
- Kubernetes
- AWS-SQS
- AWS-SES

#### Overall Design

![image-20221206023919326](https://tva1.sinaimg.cn/large/008vxvgGgy1h8tght890uj30zk0hrjsy.jpg)

##### Gateway
- Gateway, responsible for routing and authentication.

##### APP SPA
- Single page application.

##### MyAccount SPA
- Employee's personal homepage.

##### Who Am I REST API
- You can view the current user information.

##### Account API REST API
- User information storage and modification module.

##### Company API REST API
- Company module, responsible for staff management and scheduling.

##### Bot REST API
- Message queue. After updating the schedule, a message is sent to the Bot.

##### Mail Sender REST API
- Fetch the message from the message queue, the consumer of the message. 

- Send email to employee email address.

##### Database
- The MySQL database



### TODO

Just a design, not yet started development, continuing
