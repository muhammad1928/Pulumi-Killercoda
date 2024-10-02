
### `step4.md` - **Deploying Your Multi-Cloud Infrastructure**
```markdown
# Step 4: Deploying Your Multi-Cloud Infrastructure

Now that you've written your Pulumi code, it's time to deploy your infrastructure.

## Step 4.1: Run Pulumi Preview
First, run a preview to see what changes Pulumi will make:

```bash
pulumi preview
```

Pulumi will show you a preview of the resources that will be created on AWS and Azure.

## Step 4.2: Deploy the Infrastructure
To deploy the resources, run:
```bash
pulumi up
```

Follow the prompts to confirm the deployment. Pulumi will create an S3 bucket on AWS and a Resource Group on Azure.

