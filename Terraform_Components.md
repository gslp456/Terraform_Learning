#In this section we shall discuss about the Terraform components

Now, Phani has got to know that Terraform can accomplish whatever he is trying to do in a very very less time. So he decided to learn it. 

Terraform can be downloaded from the hashicorp terraform official website.

We will write the terrafrom related configuration in JSON or Yaml. 

The language which we use to write the Terraform file is call Hashicorp Language (HCL)

Before we get to writing these, we need to know how to define infrastructure and how Terraform can identify what we need it to accomplish.

Terraform has several components that can be utilized to build the Infra/Automate/Maintain the state etc.

	> Providers
	> Resources
	> Variables
	> Statefiles
	> Provisioners
	> Backends
	> Modules
	> Datasources
	> Service Principals

Providers:

Providers are the plugins that Terraform uses to communicate to respective platform where we are intended to build and configure the infrastructure. For instance, Phani wanted to provision the infrastructure on Azure cloud platform. So, he will use the Azure related provider through which Terraform will know on which platfrom it needs to create the instances and also under this Azure provider (Azure Resource Manager) - we will configure the authentication details and also the region where it is hosted. Without providers, we will not be able to perform anything because Terraform is lost without it.
Example:


	Provider "azurerrm" {
	version = "~2.0"
	   features {}
	   subscription_id =
	   client_id =
           client_secret =
	   tenant_id =
	}




Resources:

Next comes the resources. We have defined provider - Now TF is able to authenticate to the Azure platfrom. Now it needs to create instances or resources , but it needs to know what type of infrastructure object it should create - such as , VNET,Subnet,Instances etc. These can be achieved through the terraform component called Resources. 
