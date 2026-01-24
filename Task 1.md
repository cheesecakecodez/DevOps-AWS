# Task 1

Configuring Jenkins Plugin for cloud provider (for auto scalable  loads)

![image.png](Images/Task%201/image.png)

![image.png](Images/Task%201/image%201.png)

![image.png](Images/Task%201/image%202.png)

![image.png](Images/Task%201/image%203.png)

![image.png](Images/Task%201/image%204.png)

![image.png](Images/Task%201/image%205.png)

![image.png](Images/Task%201/image%206.png)

![image.png](Images/Task%201/image%207.png)

![image.png](Images/Task%201/image%208.png)

![image.png](Images/Task%201/image%209.png)

![image.png](Images/Task%201/image%2010.png)

![image.png](Images/Task%201/image%2011.png)

2 plugins used amazon ec2 and ssh agent plugin 

pipline-

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

[](https://www.notion.so/2f2e31ead61080019833de44afe5ee8f?pvs=21)
