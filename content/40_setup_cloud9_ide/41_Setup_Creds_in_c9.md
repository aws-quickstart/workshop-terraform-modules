+++
title = "Setup AWS Credentials"
chapter = true
weight = 41
+++

## In Cloud9 Terminal

Run `aws configure`

{{% notice tip %}}
Copy the values for **AWS ACCESS KEY ID** and **AWS SECRET ACCESS KEY** from the AWS IAM Console. If you have accediently closed this tab you can find the credentials in the csv file that you downloaded in the **Getting Started** Section.
{{% /notice %}}

- Set: AWS ACCESS KEY ID < Copy and Paste

- Set: AWS SECRET ACCESS KEY < Copy and Paste

- Set:Default REGION NAME to : us-west-2

- Set: Default OUTPUT FORMAT to : None (Just hit enter)

_Expected Output:_
![aws-creds1](/images/aws_creds1.png)

### Add AWS_REGION Variable to bash_profile

```
echo "export AWS_REGION=us-west-2" | tee -a ~/.bash_profile
export AWS_REGION=us-west-2
```

### Validate the IAM user

Use the __GetCallerIdentity__ cli command to validate that the Cloud9 IDE is using the correct IAM user.

```
aws sts get-caller-identity
```

_Expected Output:_
![aws-creds2](/images/aws_creds2.png)


{{% notice tip %}}
Leave Cloud9 open we will be using cloud9 through out this workshop
{{% /notice %}}





