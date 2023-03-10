# AFT-Udemy

- [AWS Control Tower](https://docs.aws.amazon.com/controltower/latest/userguide/what-is-control-tower.html)

- [AFT](https://docs.aws.amazon.com/controltower/latest/userguide/taf-account-provisioning.html)
- [AFT-Architecture](https://docs.aws.amazon.com/controltower/latest/userguide/aft-architecture.html)
- [Costing](https://docs.aws.amazon.com/controltower/latest/userguide/aft-pricing.html)
- [Deployment](https://docs.aws.amazon.com/controltower/latest/userguide/aft-getting-started.html)

## Section-1 Introduction

- AWS Control Tower Account Factory for Terraform (AFT) follows a GitOps model to automate the processes of account provisioning and account updating in AWS Control Tower. You'll create an account request Terraform file, which provides the necessary input that triggers the AFT workflow for account provisioning.

When account provisioning or updating is complete, the AFT workflow continues. It runs the AFT account provisioning framework and account customizations steps.

    - Note
        - AFT does not affect workflow performance in AWS Control Tower. For example, if you provision an account through Account Factory, or through AFT, the same backend workflow occurs, without any timing differences. AFT enables automation, therefore the time required for provisioning may be less noticeable.

### Requirements

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

### Organizations Structure

- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221487359-10251216-30d5-48a0-beda-f78541d90903.png)

- ![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/57224583/221487537-035bdbbb-7e6b-4ed5-b704-61c872163f0e.png)

- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221488417-d4bc6903-7d31-48ff-82f8-24d73aecbf9c.png)

- ![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/57224583/221488459-e9210322-21f6-440e-8d49-478ab34feec1.png)

### Master Account

- it is also called Organization master account, which manages the organization.

  - manages OU Structure
  - create aws accounts
  - invite other existing accounts
  - remove accounts
  - apply policies

- Master account should only be used for:

  - stackset
  - org details
  - scp policies
  - sso configuration
  - biling data

- Do not apply SCP to the root of ypur organization
- use the Private group-mail address.
- Use Complex Passwords with 2FA
- limit Access
- Monitor Activity
- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221490617-dc4374e2-5665-406e-bb5c-939bb4734239.png)
- ![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/57224583/221490687-e7fb31a7-7a13-46c4-bce7-db14f6d1fca1.png)

### Security & Control

- [Security](https://docs.aws.amazon.com/controltower/latest/userguide/security.html)
- [Controls](https://docs.aws.amazon.com/controltower/latest/userguide/controls.html)

- ![MicrosoftTeams-image](https://user-images.githubusercontent.com/57224583/221501212-d6196c08-2cc3-49be-952e-1f084c2dad24.png)
- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221501349-14e677c7-9211-4aee-a01e-9671333c4bd3.png)
- ![MicrosoftTeams-image (2)](https://user-images.githubusercontent.com/57224583/221501400-6a5b5122-4f0b-4fa7-95a9-8e40d573e3c4.png)
- ![MicrosoftTeams-image](https://user-images.githubusercontent.com/57224583/221501581-885c7191-92fd-48cd-bc4a-6cc2912b584e.png)
- ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/221501638-1150f6da-71fc-4873-99a1-33d0cfba2fb7.png)

### Accounts Concept (Network Account)

- [Networking Account](https://docs.aws.amazon.com/managedservices/latest/userguide/networking-account.html)

  - ![MicrosoftTeams-image](https://user-images.githubusercontent.com/57224583/222044821-3c387efc-1c75-4378-82d2-673379188e2e.png)
  - ![MicrosoftTeams-image (1)](https://user-images.githubusercontent.com/57224583/222045329-52d9c4f7-308f-43ea-93f3-c6e613c1abe3.png)
