
1- Install serverless:

      npm install -g serverless

    Set up a new user in IAM named "serverless" and save the access key and secret key.

2- Configure serverless to use the AWS credentials you just set up:

     sls config credentials --provider aws --key YOUR_ACCESS_KEY --secret YOUR_SECRET_KEY --profile serverless

To get a list of the available serverless templates run:

     sls create --template

To create a serverless boilerplate project:

     sls create --template aws-nodejs-typescript --path 10-udagram-app

To deploy the application:

 Install the dependencies:

       npm install

  Deploy the application

     sls deploy -v

Note: if you get a permissions error when you run deploy you may need to specify the user profile

     sls deploy -v --aws-profile serverless

to Automatically deleting preview deployments:

     sls remove

