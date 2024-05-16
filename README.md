# ecommerce-cloud-native-app
Objectives:
Demonstrate the robustness of our architectural framework by simulating an application environment using application hosted on AWS. This experiment aims to showcase the effectiveness of the proposed architecture in handling high traffic conditions, ensuring scalability, and adhering to best practices for availability and monitoring

### AWS CloudFormation Template:
Develop a CloudFormation template of the mock application to represent the proposed architecture. 
Include configurations for EC2 instances, Auto Scaling, Load Balancer, and CloudWatch.

### Load Balancer Configuration: 
Set up the Load Balancer to evenly distribute incoming traffic across multiple EC2 instances. See Fig for reference to Load Balancer setup for your experiment
Configure to operate across different availability zones for enhanced reliability.

![lb](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/a9816b9e-9d8a-44cc-8c18-17258529fbf5)

### Auto Scaling Integration: 
Integrate EC2 Auto Scaling to adjust resources based on traffic patterns and demand.

### AWS CloudWatch Setup: 
Configure AWS CloudWatch for real-time monitoring of the hosted application. 
Set up custom metrics and alarms to trigger notifications in case of threshold breaches.

![cloudwatch](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/fd5af244-7a26-4ed6-9b53-61daab98fa60)


### Testing Under High Traffic Conditions: 
Simulate high traffic conditions with Locust to observe the Load Balancer efficiently distributing workloads. Refer to Fig below for Locust workload generation.
Monitor the system's response to scaling events triggered by Auto Scaling policies.

### Alarm Testing: 
Intentionally trigger threshold breaches to validate responsiveness of configured Alarms. 
Ensure timely notifications and responses to deviations from expected performance.

## Workload Generation With Locust

In our specific experimental setup, we leverage a consistent high-traffic workload to assess the application's ability to handle heavy loads.This approach ensures a thorough examination of the application's resilience and scalability under demanding conditions.

![locust](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/ac0e6715-7487-4737-8439-b497a346c973)


## Analysis of Results

### CPU Utilization of Main Application:
![cpu](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/84edfc63-80cb-4446-a7ee-aee191e1161e)


### NetworkPacketIn of Single Instance Application:

![net](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/125f680a-10ec-4c99-a738-e6ae9c1682fa)


###  Multiple Instance with Load Balancer Analysis
![re](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/c0435d40-c102-4db1-8c9c-7a0b6c47cf18)



![f](https://github.com/Pradeep23-01/ecommerce-cloud-native-app/assets/66003584/10ff8282-39a9-4100-bf3e-111ec5d7418d)



