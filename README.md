# 4640-w13-lab-start-w25

For our terraform configuration to work you need a prebuilt s3 bucket to use as the backend. 

Once the s3 bucket is created we can add it to the terraform configuration provider.tf using a backend block. 

Once configuration file is configured, run the following commands:

```
terraform init

terraform plan

terraform apply
```

when is the state file created?

Created during terraform apply and available until removed. 

When is the lock file present?

Created and available during the apply and plan process, unavailable after the terraform configuration is executed.

Is the lock file always in the bucket after it is created?


No, the file is temporary and is removed from the bucket after terraform apply is done executing.
![Screenshot 2025-04-04 145338](https://github.com/user-attachments/assets/6bd004c0-300c-4e39-b026-ea2bfc5d0cf0)
![Screenshot 2025-04-04 150308](https://github.com/user-attachments/assets/43de60c7-16dc-4849-bcd4-5b5e2337292f)
