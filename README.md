# AFT-Udemy

## Section-1 Introduction

- AWS Control Tower Account Factory for Terraform (AFT) follows a GitOps model to automate the processes of account provisioning and account updating in AWS Control Tower. You'll create an account request Terraform file, which provides the necessary input that triggers the AFT workflow for account provisioning.

When account provisioning or updating is complete, the AFT workflow continues. It runs the AFT account provisioning framework and account customizations steps.

    - Note
        - AFT does not affect workflow performance in AWS Control Tower. For example, if you provision an account through Account Factory, or through AFT, the same backend workflow occurs, without any timing differences. AFT enables automation, therefore the time required for provisioning may be less noticeable.

## Requirements

- Experience

  - Foundational Knowledge of AWS
  - Basic Linux Commands

- Resources
  - AWS Account
  - Windows / linux/ mac os machine
  - pre-installed GIT and GITHUB Account

## Section-2 Landing Zone Concept

- ![lz-1](https://user-images.githubusercontent.com/57224583/221477458-22c73864-99f9-44e4-ace7-b526e1654a51.png)

- ![lz](https://user-images.githubusercontent.com/57224583/221477543-794ac104-dba7-4917-9981-02486586057e.png)

- Using the landing zone, you can split your workloads on the different accounts, but in fact still manage them from the centralized place. Like in this example, you can make different kind of accounts which will be responsible for the specific job on your mechanism.
- You can have separated accounts per your application or have split on the development or for the client view accounts, the actual separation you can choose by yourself, and even then they still will be able to use same resources.
- You can easily share them between the same for the security and the login part. You can have distinct accounts responsible for this.
- They will monitor all your activity across account and applications there and collect all information on one centralized place which is secured and hiding from all.
- Sounds good.

- Yeah, but this is not all on case of segregation, of duties.
- The landing zone helps a lot because you will have one place for the indemnification and authorization.
- This gives to you the additional layer of the security and audit.
- But as well you can control the permissions for your team and allow use only permitted resources.
- On the business side, the landing zone also can help.
- You don't need to manage the course for each account in the landing zone.
- You can have only one account which will be responsible for this and from where you can monitor and control your expenses, I think right now we are ready to give the landing zone definition.
- Landing zone is multi account architecture solution.
- The result of this have well architected framework means collect inside the latest best practice of architecture solutions.
- The possibility to scale in cup using the free account structure.
- The security governance is due to centralize in place for monitoring and logging.
- Then the define management using the elastic management permission system, the flexibility to allow engineers to simplify their development process and the business compliance because the elasticity of building management properties, all of this is the landing zone

## Section 3: AWS Landing Zone and best practices overview

- Organizations Structure
- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221487359-10251216-30d5-48a0-beda-f78541d90903.png)

- ![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/57224583/221487537-035bdbbb-7e6b-4ed5-b704-61c872163f0e.png)
