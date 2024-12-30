---
title: Setup new Project
description: Description how to bootstrap a new project
draft: true
tags:
  - GitHub
---
# Initialize new GitHub Repo
## Steps to initialize repo/project
### GitHub Repo
1. Create new (probably private) repository at [New repository](https://github.com/new)
2. Copy link to repository
3. Open a new window in Visual Studio Code
4. Using option "Clone Git Repository..." select the new repo
5. Select ```Programmieren```folder (i.e. the parent folder) to clone the repo
6. Validate that the repo is locally available at ```Programmieren\<repo_name>```
### .gitignore file
1. Go to ```gitignore.io```to create an initial .gitignore file
2. A good starting point for my stack (Azure, Azure Functions, Python with Visual Studio Code on macOS) is ```https://www.toptal.com/developers/gitignore/api/macos,azurefunctions,azurite,python,visualstudiocode```
3. Save this as ```.gitignore```
4. 
## Initial Structure
### Azure Function

### Terraform
Currently, I have one Repo that contains my TF Setup (link and page with external storage of tfstate and my logic behind it, deployment done from each subdirectory)
1. Create a new directory from template folder:
	1. Copy and paste ```tf-template```
	2. Rename to ```tf-<project>```
2. Rename ```rename_to_terraform.tfvars_file```to ```terraform.tfvars```
3. Rename ```rename_to_main.tf```to ```main.tf```
4. Adjust newly created files
	1. In ```main.tf```adjust 
	      ``` bash
		   key = "tf-<project>.tfstate"
	   ``` 
	   and populate the ```client_id```, ```tenant_id```etc. fields.
	   These are empty in the template, because the files from the template are in the repo while ```main.tf``` is part of the local ```.gitignore```to avoid these secrets being published on GitHub.

	2. In ```terraform.tfvars```likewise populate
	   ```shell
		azure_deploy_client_id = ""
		azure_deploy_client_secret = ""
```
5. Define the desired resources in ```ressources.tf```
6. ```terraform init```(this will also initialize the state store in Azure)
7. ```terraform plan```
8. ```terraform apply -compact-warnings```
More details in [[[Terraform - FunctionApp Template]]].
