#### EC2 (Elastic Compute Cloud)

- ```aws ec2 run-instances --image-id <image_id> --instance-type <instance_type> --key-name <key_pair_name>```: Launch an instance.
- ```aws ec2 describe-instances```: List instances.
- ```aws ec2 terminate-instances --instance-ids <instance_id>```: Terminate an instance.

#### S3 (Simple Storage Service)
- ```aws s3 ls```: List buckets.
- ```aws s3 cp <file_path> s3://<bucket_name>/<destination>```: Upload a file. 
- ```aws s3 cp s3://<bucket_name>/<file_key> <destination>```: Download a file. 
- ```aws s3 rm s3://<bucket_name>/<file_key>```: Delete a file.

#### IAM (Identity and Access Management):
- ```aws iam create-user --user-name <username>```: Create an IAM user. 
- ```aws iam list-users```: List IAM users.
- ```aws iam attach-user-policy --user-name <username> --policy-arn <policy_arn>```: Attach a policy to a user.
