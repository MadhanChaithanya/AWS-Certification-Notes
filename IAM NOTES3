### Writing Simple IAM Policies:
For Grammar Refer Here:

https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_grammar.html


### S3 Bucket Use-Cases:
1) Give Permissions to the user for S3(Service Level Access)
2) Deny Permissions to the user on some bucket(Resource Level Access)
3) Give Permission to the user on S3 to read but not to write or delete or create

If your company is using Service Level Access means Amazon Managed Polices are enough.
eg: 
EC2 Read Only Access
EC2 Full Access

If your company is using Resource Level Access means Customer Managed Policies are used.

### Service Level Policies:
- It applies to all the resources under that service. (Consider Use case 1)
- For every AWS resource, we have an unique ARN and in the case of service level access I can assume resource as * (AnyThing)
- Usecase 3 Speaks about Service Level Access, but there are action based Restrictions.

### Terms to Understand:
```
-> Service	- Whatever AWS offers
-> Resource	- Whatever user create
-> Actions	- What can you do on that resources  i.e, different operations of Resource
eg:
- From S3 I can create a file or delete a file.
- I can give public permission or I cannot give public permission.
```
For every resource you have this.

- Whenever you're writing an IAM Policy all of these 3 come into play.
- If you're writing an Service Level Access and if you're speaking about all the actions - your Resources and Actions will be *.

When you're speaking about specific stuff or it will be something else and Actions will be something else.

For this IAM you don't need to have a knowledge on AWS.

### Considerations to Write Policy: 
What are the things you need to consider while writing an policies:
1. Policy Grammer.
2. Which service are you writing the plicy around.
3. Is the Resource Specific.
4. What are all the possible actions of this resource.


IAM Policy for Usecase-1:
* To Get all the actions google ``` aws iam <service> actions ```, in this case i will be querying with ``` aws iam s3 actions ```
```
{
    "Version" : "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": ["s3:*"],
            "Resource": "*"
        }
    ]
}
```
* To give Readonly access add the necessary actions to Statment => Action List
```
 {
    "Version" : "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": ["s3:Get*","s3:Describe*","s3:List*"],
            "Resource": "*"
        }
    ]
}
```
* To Give Readonly on one resource and write on all others
* First findout ARN for that Resource. ```aws s3 arn  ```
* Test this for read only on one bucket
```
{
    "Version" : "2012-10-17",
    "Statement": [
        {
            "Resource": "arn:aws:s3:::bucket_name",
            "Effect": "Deny",
            "Action": ["s3:AbortMultipartUpload", "s3:Create*", "s3:Delete*", 
            "s3:ObjectOwnerOverrideToBucketOwner", "s3:Put*", "s3:Replicate*","s3:Restore*"] 
        },
        {
            "Effect": "Allow",
            "Action": ["s3:Get*","s3:Describe*","s3:List*"],
            "Resource": "*"
        }
    ]
}
```























