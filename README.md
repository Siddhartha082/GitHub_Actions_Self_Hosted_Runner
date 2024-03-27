# GitHub_Actions_Self_Hosted_Runner on AWS EC2 Instances

Repository to kick start your journey with GitHub Actions

## Comparing with Jenkins 

### Advantages of GitHub Actions over Jenkins

- Hosting: Jenkins is self-hosted, meaning it requires its own server to run, while GitHub Actions is hosted by GitHub and runs directly in your GitHub repository.

- User interface: Jenkins has a complex and sophisticated user interface, while GitHub Actions has a more streamlined and user-friendly interface that is better suited for simple to moderate automation tasks.

- Cost: Jenkins can be expensive to run and maintain, especially for organizations with large and complex automation needs. GitHub Actions, on the other hand, is free for open-source projects and has a tiered pricing model for private repositories, making it more accessible to smaller organizations and individual developers.

### Advantages of Jenkins over GitHub Actions

- Integration: Jenkins can integrate with a wide range of tools and services, but GitHub Actions is tightly integrated with the GitHub platform, making it easier to automate tasks related to your GitHub workflow.

In conclusion, Jenkins is better suited for complex and large-scale automation tasks, while GitHub Actions is a more cost-effective and user-friendly solution for simple to moderate automation needs.

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/6c453711-b216-4450-9871-ea12df4d1019)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/d9a4dff7-0d75-4d73-b9d4-a0430726cbfd)

Github Actions Self Hosted Runners.

- What is Self Hosted Runners ?
- 
A self-hosted runner is a system that you deploy and manage to execute jobs from GitHub Actions on GitHub.com.
For more information about GitHub Actions, see "Understanding GitHub Actions.

- Advantages of using Self Hosted Runners ?
  
Control Over Execution Environment:
Cost Efficiency:
Increased Security:
Reduced Latency:
Compatibility:
Scalability:
Offline Workflows:
Resource Limits and Quotas:

-step by Step Demo to write your first GitHub Actions CI using the Self Hosted Runners. 

Certainly! Below is a simple example of a GitHub Actions workflow file 
.github/workflows/ci.yml that utilizes self-hosted runners. This workflow will run on
every push to the repository and execute a  simple build script on the self-hosted runyamlner:

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/3aec4ff7-babf-4157-bf02-df7ea150a902)


# Yaml file

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/606e50a7-f546-4847-a7a5-d88824a55b9d)

# - EC2 instance as Self Hosted Runners ?

-- lets see this Practically below

# Aws Console

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/a0ca4ed3-39da-4ae8-856d-abdf697f8414)

# inside EC2

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/8c0fc134-4602-47e9-b930-eaf7654186fe)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/90eee7a9-fdda-48e3-a336-1bbd8ba47c72)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/3453c4b1-b2f7-46b0-a425-287c1f1faaf3)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/7c702be8-ec42-462f-b189-f9570d65f781)

# Keypair- Authentication for SSH console 

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/a69ca94a-f505-4be7-a6f6-1626eb7b9488)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/acad8b10-f55e-4f60-8f03-27c6fda33e5b)

# note -configure inbound / Outbound traffic rules in security groups 4 communication

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/b5b6ab6f-1fa5-448e-8086-a9b59be65f2f)

# Edit inbound rules

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/32aec2be-d321-4731-9ce2-a5d23d316db1)

# Edit Outbound rules

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/7757ca9c-770a-4195-b7ec-a6ece0a6b2d5)

# My repo - https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner_On_AWS_EC2_Instances

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/b6c78835-86d0-4c61-ad5c-807ce4422527)

# Yaml File

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/edc0de97-4b4c-4d45-ab18-30cb71e29352)


# As soon as change made to the repo

# Commit

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/b827b39e-c275-4125-8747-943e2bb50ac3)

# the tick mark  shows GitHub Actions Successful & Verified

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/c72577cd-7a65-4541-896e-fd110062893d)

# now Fix to Self Hosted Runner

# go to Setting Tag .. Click & select Actions – select Runner 

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/a357ff47-727f-4734-b096-464075523e3e)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/6f201522-a16a-40af-ab76-b2c580c1f386)

# Click on New Self hosted runner

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/9e9a5bf7-565c-4961-8293-cfb5de2d69c8)

# Steps to be Followed

# Connect to  EC2 through ssh session using MobaXterm Client

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/89bde8d5-c758-4c60-9b50-a01d7d980a49)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/74790617-82f9-4988-a574-e4fcb931a008)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/f07419b1-dada-466e-81ee-474da4409d8b)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/3d44ae24-21df-4cb6-acad-5432536f567b)

# Go To repo  @ Yaml file – Edit the Page

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/f3105f86-47e2-47a0-af52-f85c7de45e49)

# change the Below in Yaml file

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/178fc2ba-810d-4f69-8d1f-c4c687af4a39)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/a6544a7c-a817-4254-ac40-63d08d1b655c)

# Commit change

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/c9a6b059-c54f-4c3b-a47e-166aac820844)

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/64627f1a-fa09-498e-909f-ab7ffbb99cad)

# Yellow  Marking

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/f484af8b-763d-422c-8a19-f55d8cd232e0)

# updated to green Tick mark -- Actions Successful 

![image](https://github.com/Siddhartha082/GitHub_Actions_Self_Hosted_Runner/assets/110781138/348fa37c-0ebe-40b7-a46c-afeca78b2a01)



