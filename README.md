# AWS SDK for Node.js Sample Project

A simple Node.js application illustrating usage of the AWS SDK for Node.js.

## Basics Requirements of AWS SDK for JavaScript in Node.js

a - Download sample project:
git clone https://github.com/DavidsonLuna/aws-nodejs-sample

b - The only requirement of this application is the Node Package Manager. All other
dependencies (including the AWS SDK for Node.js) can be installed with:

    cd aws-nodejs-sample
    npm install

## Basic Configuration

You need to set up your AWS security credentials before the sample code is able
to connect to AWS. You can do this by creating a file named "credentials" (without extension) at ~/.aws/ 
(Users/USER_NAME/.aws\credentials for users Mac/Linux) and saving the following lines in the file:

    [default]
    aws_access_key_id = <your access key id>
    aws_secret_access_key = <your secret key>

OBS.:
* Remember that the .aws directory is a system file, ie hidden. To view run ls -la
* To create the directory .aws run: mkdir .aws
* To create the directory credentials: touch credentials (without extension)
    
See the [Security Credentials](http://aws.amazon.com/security-credentials) page.
It's also possible to configure your credentials via a configuration file or
directly in source. See the AWS SDK for Node.js [Developer Guide](http://docs.aws.amazon.com/AWSJavaScriptSDK/guide/node-configuring.html)
for more information.

## Running the S3 sample

This sample application connects to Amazon's [Simple Storage Service (S3)](http://aws.amazon.com/s3),
creates a bucket, and uploads a file to that bucket. The script will automatically
create the file to upload. All you need to do is run it:

    node sample.js

The S3 documentation has a good overview of the [restrictions for bucket names](http://docs.aws.amazon.com/AmazonS3/latest/dev/BucketRestrictions.html)
for when you start making your own buckets.

------------

## Writing Unit Testing:

To create the directory for unit test run:

    mkdir sls-unit-test

To access the directory:

    cd sls-unit-test

To create the template:

    sls create --template aws-nodejs --name sls-unit-test

To create the init:

    npm init -y

------------
## Additional Resources
For detailed user guides, API documentation, developer forums, and other developer resources, see the AWS SDK for JavaScript page at Node.js.

## License

This sample application is distributed under the
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).


