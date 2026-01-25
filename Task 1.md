# Task 1

Configuring Jenkins Plugin for cloud provider (for auto scalable  loads)


Enables you to use Jenkins to rum an AWS EC2 instance.  So those who are new to Jenkins is an open source platform which is used to do repetitive jobs  are development , it is a major part of CI/CD . So one real life use case- you are making a project you setup a set of fixed constraints and acceptable outputs for ensuring the working of the project. So set a number of tests. Here’s were setting up a job on Jenkins comes in handy it can trigger the run of tests on the set of codes then work according to the output - more info in the AWS-Jenkins repo.

Integrating it with a cloud service allows you to scale your work at lower costs and efficiently 

Here are the steps of how I did it:-

Step 1.  Make an EC2 instance EC2→Instance

![image.png](Images/Task%201/image.png)

Step 2. Make  a key-pair it is the best practice to use key-pair to ensure security of data and work.

![image.png](Images/Task%201/image%201.png)

Step 3. Change 0.0.0.0/0 to you IP because you don’t want unwanted visitors. There’s is no need of HTTP traffic here we will use Jenkins only for this task.

![image.png](Images/Task%201/image%202.png)

Step 4. Click create Instance EC2 instance will start running.

![image.png](Images/Task%201/image%203.png)

Step 5. Check that you able to connect your linux(debian) kernel to this instance using the keypair you generated. command ssh -i <keyname>.pem ec2@<public IPv4 address of your EC2 instance 

![image.png](Images/Task%201/image%204.png)

Step 6. Login to your Jenkins. Navigate to Jenkins→Manage→Security→Credentials

![image.png](Images/Task%201/image%205.png)

Step 7.  Tricky part Under “Store scoped to Jenkins” → under “domain” click on “(global)”  click add credentials and you will reach →

![image.png](Images/Task%201/image%206.png)

Step 8. Select “Username with Private key” as the kind.  Don’t change scope. 

Under ID type the the name for credentials in Jenkins you will refer to the created instance with this.  Enter ec2-user as Username because  in Step 1 the Amazon Machine Image was selected as Amazon Linux.

 [Use → admin if AMI was selected as Debian] click enter directly.

![image.png](Images/Task%201/image%207.png)

Step 9. On your terminal cat <your-aws-key>.pem to get key as output . Copy and paste it in the key box. This will enable you to connect the EC2 .  Key will be created.

![image.png](Images/Task%201/image%208.png)

Step 10. Create a job pipeline to test the connection with instance , make sure your instance is up and running.

![image.png](Images/Task%201/image%2010.png)

![image.png](Images/Task%201/image%2011.png)

 Click On build now done
2 plugins used amazon ec2 and ssh agent plugin 

YAYYYYY

console output-

Started by user Suhani Nagwani

[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins
in /var/lib/jenkins/workspace/ec2-ssh-test
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Init)
[Pipeline] sshagent
[ssh-agent] Using credentials ec2-user (Configuring in aws. Cloud Provider)
$ ssh-agent
SSH_AUTH_SOCK=/tmp/ssh-8u1Pe19inOEu/agent.22339
SSH_AGENT_PID=22344
Running ssh-add (command line suppressed)
Identity added: /var/lib/jenkins/workspace/ec2-ssh-test@tmp/private_key_10445153240618770606.key (/var/lib/jenkins/workspace/ec2-ssh-test@tmp/private_key_10445153240618770606.key)
[ssh-agent] Started.
[Pipeline] {
[Pipeline] echo
SSH credential loaded
[Pipeline] }
$ ssh-agent -k
unset SSH_AUTH_SOCK;
unset SSH_AGENT_PID;
echo Agent pid 22344 killed;
[ssh-agent] Stopped.
[Pipeline] // sshagent
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
Finished: SUCCESS

Local Jenkins Configuration into ec2

