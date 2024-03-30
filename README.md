# Project Title: Infrastructure for tycrowe.com

## Project Summary:
This project is the infrastructure for tycrowe.com. It is a static website hosted on AWS S3 and CloudFront. The infrastructure is defined using Cloudfront.

## Deployment:
To install the infrastructure, you will the AWS CLI installed and configured with the appropriate permissions. 
1. Start by cloning the repository.
2. Use the AWS CLI to create the local stack for the /shared/buckets.yml file first:
```aws cloudformation create-stack --stack-name <name>-shared --template-body file://shared/buckets.yaml```
3. Pick a component to install. For example, to install Codefolio:
```aws cloudformation create-stack --stack-name <name>-codefolio --template-body file://codefolio/codefolio.yaml```

## Live Site:
The live site can be found at [tycrowe.com](https://tycrowe.com)

## Authors:
- **Tyler Crowe** - *Core Maintainer* - [tycrowe](https://tycrowe.com)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.