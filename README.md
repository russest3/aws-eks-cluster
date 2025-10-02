# Build out a Kubernetes Cluster in an AWS VPC with Cloud Development Kit!

To Update kubeconfig:

```
aws eks update-kubeconfig --name custom-eks-cluster
```

## Architecture

![](images/aws-vpc.drawio.png)

## Requirements

- AWS CDK installed
- AWS CLI installed
- Run `aws configure` to configure access keys


## AWS CDK Procedure

Create a virtualenv on MacOS and Linux:

```
$ python3 -m venv .venv
```

After the init process completes and the virtualenv is created, you can use the following
step to activate your virtualenv.

```
$ source .venv/bin/activate
```

Once the virtualenv is activated, you can install the required dependencies.

```
$ pip install -r requirements.txt
```

At this point you can now synthesize the CloudFormation template for this code.

```
$ cdk synth
```

Deploy the IaaC code with:

```
$ cdk deploy
```

## Useful commands

 * `cdk ls`          list all stacks in the app
 * `cdk synth`       emits the synthesized CloudFormation template
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk docs`        open CDK documentation

Enjoy!
