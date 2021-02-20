# S3-simple storage service.
#In s3 files are called as objects.
# we can store unlimited data in a bucket.but object size should not exceed more than 5TB(5tera bytes).
#In each insatnce we can create only 100 buckets.
# in free tier account you get 5gb storage for free/month.

Creating a bucker:
under s3-->goto create bucket-->region-->we can eanble or disable  block public access checkbox -->tag(optional)-->versioning (optional)-->default encryption-->click on create bucket.

*bucket name should be unique.
* only two spl characters are allowed. those are - and . This should be in the middile of the name.
* length 3-63characters
* lowercase leeters only
* numerics also allowed

* Now we can upload objects by upload option under bucket.

#permissions:
mainly we need to nedd to know 3 permissions
1)Block public access (bucket settings)
Public access is granted to buckets and objects through access control lists (ACLs), bucket policies, access point policies, or all. In order to ensure that public access to all your S3 buckets and objects is blocked, turn on Block all public access. These settings apply only to this bucket and its access points
2)Bucket policy
The bucket policy, written in JSON, provides access to the objects stored in the bucket. Bucket policies don't apply to objects owned by other account.

#how to create bucket policy:
first select the bucket-->go to permissions -->bucket policy-->Edit-->policy generator
unser policy generator
->select policy type
->generate bucket policy and paste under edit bucket policy and save chages

