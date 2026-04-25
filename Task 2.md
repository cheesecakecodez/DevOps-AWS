# Task 2

Create an ec2 instance

install nginx on istance

browse the browser

1. Go EC2 → Instances. Select launch instance

![image.png](Images/Task%202/image.png)

1. Write name of instance ,add the shh key and also save it if creating new, This is a simple tutorial so leave security group and networking settings as it for now.

![image.png](Images/Task%202/image%201.png)

1. Click on instace ID, In the lower menu select Security→ click on the security group ID

![image.png](Images/Task%202/image%202.png)

1. Click on edit inbound rules, set http as 0.0.0.0(anywhere) and ssh to your ip address(custom).

![image.png](Images/Task%202/image%203.png)

1. Click on save rules.

![image.png](Images/Task%202/image%204.png)

1. Now that inbound rules are changed. Move to instance id again and click Connect.

ssh -i "awskey.pem" [ec2-user@ec2-3-253-114-187.eu-west-1.compute.amazonaws.com](mailto:ec2-user@ec2-3-253-114-187.eu-west-1.compute.amazonaws.com)

![image.png](Images/Task%202/image%205.png)

7.copy the ssh command from here paste it in your terminal. On entering you will enter your ec2 instance →It is up and running.

![image.png](Images/Task%202/image%206.png)

8. Check for updates after updating yum sudo yum update -y. These commands vary from environment to environment. for example it is apt in Debian.

1. Install nginx “sudo yum install nginx -y”.

![image.png](Images/Task%202/image%207.png)

9. After installing is Complete. Start the nginx service

- sudo systemctl start nginx [start nginx service]
- sudo systemctl enable nginx [enable the nginx service]
- sudo systemctl status nginx [check the status of your nginx server]

![image.png](Images/Task%202/image%208.png)

1. Now that it is up and running, type your ip in your browser → It will show welcome to nginx.

![image.png](Images/Task%202/image%209.png)

![image.png](Images/Task%202/image%2010.png)

1. Change the ssh to 0.0.0.0 for the ease of task. It all comes down to who has the access to we added to the instance on creation.

![image.png](Images/Task%202/image%2011.png)

1. Click on connect go to EC2 instance Connect and click on connect. You will see your instance up and running in AWS itself.

![image.png](Images/Task%202/image%2012.png)
