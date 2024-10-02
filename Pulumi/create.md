<!-- ### Create a project on TypeScript

To create a new pulumi project and to be able to edit the proiject using typescript.

we need to run this on terminal
>mkdir quickstart && cd quickstart 
>pulumi new gcp-typescript -->



Create a project

### `step3.md` - **Writing Pulumi Code for Multi-Cloud Resources**
```markdown
# Step 3: Writing Pulumi Code for Multi-Cloud Resources

In this step, you will write a Pulumi program that deploys infrastructure on both AWS and Azure.

## Step 3.1: Initialize a New Pulumi Project
Start by initializing a new Pulumi project in Python (you can also use TypeScript):

```bash
pulumi new aws-python
```

Follow the prompts to complete project initialization.

## Step 3.2: Write Pulumi Code for AWS
Edit the generated __main__.py file and add the following code to create an AWS S3 bucket:

```bash
import pulumi
import pulumi_aws as aws

# Create an AWS S3 bucket
bucket = aws.s3.Bucket('my-bucket')

# Export the bucket name
pulumi.export('bucket_name', bucket.bucket)
```

## Step 3.3: Write Pulumi Code for Azure
Next, add the Azure resources to the same file:

```bash
import pulumi_azure as azure

# Create an Azure resource group
resource_group = azure.core.ResourceGroup('my-resource-group')

# Export the resource group name
pulumi.export('resource_group_name', resource_group.name)

```