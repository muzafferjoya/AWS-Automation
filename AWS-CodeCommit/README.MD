
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

 $ echo '<h6> HelloWorld! </h6>' > index.html

 $ git status

 $ git add .

 $ git commit -m 'new' index.html

 $ git push origin master
 
