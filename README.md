# mvcproject
[![Build Status](https://dev.azure.com/AzureOrganization-git/ProjectRepo/_apis/build/status/First-Mvcapp.CI?branchName=master)](https://dev.azure.com/AzureOrganization-git/ProjectRepo/_build/latest?definitionId=1&branchName=master)

How to create this project:

git clone https://github.com/AzureOrganization-git/mvcproject.git
dotnet new mvc -au none
dotnet restore
dotnet run

git add .
git commit -m <commit message>
git push

azure devops setup:
create an org and project in azure devops, if possible with the same name as github org and project.

creating pipeline using az cli:
az login
az pipelines create --name "First-Mvcapp.CI"
az pipelines show  --name "First-Mvcapp.CI" --output table
az pipelines run  --name "First-Mvcapp.CI"
  
