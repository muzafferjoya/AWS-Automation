
### In this Project we cover

#### Introducing AWS CodeCommit - Amazon managed SAAS Git
#### Getting started with CodeCommit for HTTP users
#### Setting up CodeCommit for SSH users using AWS CLI
#### Applying security and restrictions
#### Migrating a Git repository to AWS CodeCommit


### Installation of Git and its implementation using Github


1. We have to install the Git package on our system

 $ yum install git

2. configure your identity

 $ git config --global user.name "Muzaffar khan"

 $ git config --global user.email "muzaffer----@gmail.com"

3. Check your setting

 $ git config --list

4. Now let's create git repo

 $ git clone https://github.com/muzafferjoya/AWS-Automation.git

 $ cd AWS-Automation

 $ ls

 $ touch index.html

 $ git status

 $ git add .

 $ git commit -m 'new' index.html

 $ git push origin master
 


### Introducing AWS CodeCommit - Amazon managed SaaS Git

#### Getting started with CodeCommit for HTTP users

### How to do it...

1. Open the AWS CodeCommit Console at https://ap-south-1.console.aws.amazon.com/codecommit/

2. Create a repo

3. Next, Open the IAM console at https://console.aws.amazon.com/iam

4. Click on Add User

5. Give IAM user a username as khan and check both the Access type 

6. Use Custom password

7. Next, Attach existing policies 

8. Search on searchbar AWSCodeCommitPowerUser policy and click on Next.

9. Post review , click on create user

10. Download credentials provided by the AWS IAM user, 

11. Click on user section. Then, click on security credentials

12. Scroll Down, section HTTPS GIT cred for AWS CodeCommit, click on Generate

 
