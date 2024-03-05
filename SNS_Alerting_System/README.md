<h1>EC2 CPU Utilization Alerting through SNS</h1>

Steps Involved:

CPU_Spike.py includes code to spike the EC2 CPU Utilization.


Created an EC2 instance.


Configure Alarms in AWS Cloud Watch console and set parameters like metrics, threshold value, and Period.


Create a SNS topic and mention the Email Address and body of the email.


Connect to EC2 instance and run CPU_Spike.py python file in it.


Monitor in the metrics section, when the spike crosses the threshold value you get a automated email from cloud watch.

