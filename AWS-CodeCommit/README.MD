
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

13. Again, let's go to the CodeCommit console and click on Clone URL and then HTTPS

14. Copy the link git clone https://git-codecommit.ap-south-1.amazonaws.com/v1/repos/HelloWorld

15. Type, Username and Password

16. Go to , HelloWorld Folder cd HelloWorld

17. ls 

18. touch index.html

19. git push origin master

20. Now, we pushed a file to our newly created repo in AWS CodeCommit. let's see the AWS CodeCommit console.



### Setting up CodeCommit for SSH users using AWS CLI

#### we will use SSH private and public keys to access the repository. We will be accessing the repository using SSH connections.

#### Let's start

1. yum install epel-release python-pip

2. pip install awscli

3. Now, let's configure AWS CLI:

4. aws configure

5. aws codecommit list-repositories

6. aws codecommit create-repository --repository-name HelloWorld --repository-description "This repo includes static page of HelloWorld"

7. aws codecommit list-repositories

#### Let's try to clone the HelloWorld repo from CodeCommit to our dev machine, we have to establish SSH auth.

1. ssh-keygen

2. cd .ssh

3. aws iam upload-ssh-public-key --user-name khan --ssh-public-key-body "ssh-rsa" 

4. vim .ssh/config

##### Host git-codecommit.ap-south-1.amazonaws.com 
##### User AKIAQ2WK4LZHVWUHTCAP
##### IdentityFile ~/.ssh/id_rsa




