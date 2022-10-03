# Azure SQL Database Migration-Based

Example of a SQL Server Migration-Based deployment that deploys to an Azure SQL Database. Which I mention in a blog post called '[Introducing the dbops PowerShell module](https://www.kevinrchant.com/2022/09/21/introducing-the-dbops-powershell-module/)'.

It contains an example YAML file that you can use as a YAML pipeline in Azure Pipelines. You can find it in the AzureDevOpsTemplates folder. In order to use it in Azure Pipelines you can either import or fork this repository into another GitHub repository, or into [Azure Repos](https://bit.ly/3s4uO77).

Afterwards, you can select the YAML file in Azure Pipelines and tailor the pipeline to suit your needs. You can find the recommended variables inside the YAML file. Avoid putting sensitive information directly into the YAML file (like your connection details). One thing I must stress here is that the password MUST be wrapped in single quotes in the secret for it to work.

You can use the logic in 'Classic Editor' instead by adding the tasks into the GUI and transferring the logic over. Alternatively, you can build an artifact for it using the 'Classic Editor' and use the 'Releases' feature for deployments. Personally, I prefer doing the deployment using a YAML pipeline.

Please note that the databases must already exist for this to work. 

This repository is provided "as is" based on the [MIT license](https://opensource.org/licenses/MIT). Basically, I am not responsible for your use of it.
