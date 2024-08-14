<h1>AWS Website Deployment Overview</h1>

<h2>Introduction</h2>
This document provides a brief overview of the AWS services utilized to deploy a website. It outlines the core components and their functionalities.

<h2>AWS Services</h2>
<h3>EC2 (Elastic Compute Cloud)</h3>
* Provides virtual servers (instances) in the cloud.
* Used to host the website's application server.
* **Command:** `aws ec2 run-instances --image-id ami-xxxxxxxx --instance-type t2.micro --key-name my-key-pair`

<h3>SG3 (Security Group)</h3>
* Acts as a virtual firewall for EC2 instances.
* Controls incoming and outgoing traffic based on specified rules.
* **Command:** `aws ec2 describe-security-groups`

<h3>WorkMail</h3>
* Provides secure email and collaboration services.
* Used for business email and productivity tools.
* **Command:** `aws workmail create-organization --organization-name MyOrganization --alias myorg.workmail.com`

<h3>VPC (Virtual Private Cloud)</h3>
* Creates an isolated network environment in the AWS cloud.
* Used to house EC2 instances and other resources.
* **Command:** `aws ec2 create-vpc --cidr-block 10.0.0.0/16`

<h3>RDS (Relational Database Service)</h3>
* Manages relational databases in the cloud.
* Used to store website data.
* **Command:** `aws rds create-db-instance --db-instance-identifier mydbinstance --engine mysql --allocated-storage 20`

<h2>Deployment Steps</h2>
1. Create an EC2 instance with the desired configuration.
2. Configure the security group to allow HTTP/HTTPS traffic.
3. Deploy the website application to the EC2 instance.
4. Set up RDS database and establish connection from the EC2 instance.
5. Configure WorkMail for email services.

<h2>Additional Considerations</h2>
* Consider using AWS Elastic Load Balancing for high availability and scalability.
* Implement AWS CloudWatch for monitoring and logging.
* Utilize AWS S3 for static content hosting.
* Explore AWS IAM for identity and access management.

<h2>Screenshots</h2>

![image](https://github.com/user-attachments/assets/0915284c-aca1-4d39-abb8-e9e205a69cdb)
![image](https://github.com/user-attachments/assets/389bbb9f-04a1-4ec9-af48-35b0681d2409)
![image](https://github.com/user-attachments/assets/2482785a-39df-4bf5-8274-546cf7b5225e)
![image](https://github.com/user-attachments/assets/9d1e8c5b-247b-4191-a181-2ad9075af7a7)
![image](https://github.com/user-attachments/assets/99904b15-5ced-41ea-a8eb-be602438b866)
![image](https://github.com/user-attachments/assets/176c6a12-c3a6-4535-9cc3-5c36b4dc3aa1)
![image](https://github.com/user-attachments/assets/da139c71-3b2d-4244-aa84-71a0eff7b7aa)
![image](https://github.com/user-attachments/assets/8b035299-8c1f-439e-a41b-314d24d4aa29)
![image](https://github.com/user-attachments/assets/ef11e950-7f59-49de-9dd8-d310a5a8e7c1)
![image](https://github.com/user-attachments/assets/0f2b3e51-64ff-4f36-9592-b0838c75913a)







Author-Jaissika Shukla <br>
For any contributions and help contact jaissikashukla@gmail.com
