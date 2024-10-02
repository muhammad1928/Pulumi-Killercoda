<!-- 
### Install Pulumi on Windows
You can install Pulumi using elevated permissions through the Chocolatey package manager

> choco install pulumi

this wil install pulumi CLI to the usual place (often $($env:ChocolateyInstall)\lib\pulumi)

to update Pulumi 

> choco upgrade pulumi


you can specify which version of pulumi you want to install by

> choco install pulumi --version <version>


### Install Pulumi on Mac

To install pulumi on macOS 

 > curl -fsSL https://get.pulumi.com | sh -s -- --version <version> -->


 # Step 2: Setting Up Pulumi in Your Environment

## Step 2.1: Install Pulumi
To install pulumi on linux you should run
```bash
curl -fsSL https://get.pulumi.com | sh
```
or 
```bash
brew install pulumi
```
for mac

You can verify the installation by running the following command:

```bash
pulumi version
```

You should see the Pulumi version installed. If successful, you are ready to proceed.

## Step 2.2: Configure AWS and Azure Providers
Pulumi uses cloud credentials to interact with cloud platforms. In this tutorial, you’ll configure AWS and Azure providers. We will use pre-configured credentials stored in the environment.

## AWS Setup
Run the following command to configure AWS as a Pulumi provider:

```bash
pulumi config set aws:region us-west-2

```

## Azure Setup
```bash
pulumi config set azure:location WestUS

```

Once both providers are set up, you are ready to write your Pulumi program. Move to the next step!