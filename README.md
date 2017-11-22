![](https://s3.amazonaws.com/aws-us-east-1/tutorial/AWS_logo_PMS_300x180.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_available.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_ingergration.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_ecryption-lock.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_fully-managed.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_lowcost-affordable.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_performance.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_scalable.png)![](https://s3.amazonaws.com/aws-us-east-1/tutorial/100x100_benefit_storage.png)

# **Amazon Elastic File System (Amazon EFS)**

## Tutorials

### Version 1.0.0

efs-t-1.0.0

---

© 2017 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be  reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.

Errors or corrections? Email us at [darrylo@amazon.com](mailto:darrylo@amazon.com).

---

### Table of Contents  
[Tutorials](#tutorials) 

[1. Create a file system](#1-create-a-file-system) 

[2. Performance](#2-performance) 

[3. Scale-out](#3-scale-out) 

---

### Tutorials

These three (3) tutorials are designed to help you better understand the performance characteristics of Amazon Elastic File System (Amazon EFS) and how parallelism, I/O size, and Amazon EC2 instance types affects file system IOPS and throughput.
#
### 1. Create a file system
This tutorial is a set of AWS Cloudformation templates that will create an Amazon EFS file system and pre-load data to grow the file system to obtain higher levels of IOPS and throughput. Throughput on Amazon EFS scales as a file system grows. Because file-based workloads are typically spiky—driving high levels of throughput for short periods of time, and low levels of throughput the rest of the time—Amazon EFS is designed to burst to high throughput levels for periods of time. Amazon EFS uses a credit system to determine when file systems can burst. File systems can be monitored using AWS CloudWatch metrics. These Cloudformation templates will also create an AWS CloudWatch dashboard, custom metrics, alarms, scheduled events, AWS Lambda function, SNS notification, and an Auto Scaling group to monitor and dynamically adjust alarm thresholds as the file system grows and shrinks.

| Tutorial | Link
| --- | ---
| **Create a file system** | [![cloudformation-launch-stack](https://s3.amazonaws.com/aws-us-east-1/tutorial/create-efs-resources/efs-tutorial-button-20171120.png)](https://github.com/aws-samples/amazon-efs-tutorial/tree/master/create-file-system) |

### 2. Performance
This tutorial is a set of scripts that will demonstrate: 1) different instance types provide different levels of network performance when accessing a file system; 2) different I/O sizes (block sizes) and sync() freqencies (the rate data is persisted to disk) effects file system throughput; 3) increasing the number of threads accessing a file system will increase IOPS and throughput.

| Tutorial | Link
| --- | ---
| **Performance** | [![cloudformation-launch-stack](https://s3.amazonaws.com/aws-us-east-1/tutorial/create-efs-resources/efs-tutorial-button-20171120.png)](https://github.com/aws-samples/amazon-efs-tutorial/tree/master/performance) |


### 3. Scale-out
This tutorial is a Cloudformation template that will create an Amazon EC2 spot fleet and download objects in parallel from an Amazon S3 bucket.

| Tutorial | Link
| --- | ---
| **Scale-out** | [![cloudformation-launch-stack](https://s3.amazonaws.com/aws-us-east-1/tutorial/create-efs-resources/efs-tutorial-button-20171120.png)](https://github.com/aws-samples/amazon-efs-tutorial/tree/master/scale-out) |

---

## Troubleshooting


For feedback, suggestions, or corrections, please email me at [darrylo@amazon.com](mailto:darrylo@amazon.com).


## License

This library is licensed under the Amazon Software License.
