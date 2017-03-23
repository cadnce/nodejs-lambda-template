# NodeJS lambda template

A template for making nodejs lambda functions from and easily deploying while solving the question "How do I keep this code under source control and easily deploy"


## Initial configuration
### AWS:
Create an aws credentials file at `~/.aws/credentials` e.g.
```
[default]
aws_access_key_id = YOUR_ACCESS_KEY_ID
aws_secret_access_key = YOUR_SECRET_ACCESS_KEY
```

The key should be generated (in the IAM) with the role `AWSLambdaFullAccess`

### Lambda specifics:
The 'role' must be populated with a role with lambda execute permissions


## Deploying:

To deploy simply:

```
gulp deploy
```


Note: There are more options available that are possible to configure in the lambda-config.js https://github.com/ThoughtWorksStudios/node-aws-lambda