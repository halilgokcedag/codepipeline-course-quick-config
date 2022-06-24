# CodePipeline-course-quick-config


### About The Project

Created this project to help other students taking the [Udemy CodePipeline Course](https://www.udemy.com/course/aws-codepipeline-step-by-step/). Cloud Playgrounds expire after some time. Also, sometimes it might be a good to start from scratch. This code helps to build some of the basic configuration used in the course.

This code creates an instance profile, a service role, an EC2 instance and aCodeCommit repository.

EC2 instance commands are covered in the user-data of the EC2 instance. However, it is still recommended to create a key pair to connect to the EC2 instance when needed. 

### Deployment
1. Clone the repository.

2. Create a new SSH key pair. See [Creating an SSH Key Pair](https://www.ssh.com/academy/ssh/keygen). Copy the created key files to the root directory of the code.

3.Update the following variables in the variables.tf file for your setup.

- Region
- Keypair
- Ami Id
- Instance Type

4. Run the Terraform init, Terraform plan and Terraform apply commandsconsecutively. After a succesful apply, see outputs for the EC2 public IP address and CodeCommit repository http url.