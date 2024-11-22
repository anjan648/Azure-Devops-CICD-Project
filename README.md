# Azure-Devops-CICD-Project
eveloped and deployed a complete end-to-end pipeline for a Node.js application.
Steps to set the infrastructure
Login to VSCode or any other IDE of your choice

Run the below commands to download the application code

mkdir day4_youtube_clone; cd day4_youtube_clone
git init
git clone https://github.com/piyushsachdeva/Youtube_Clone
Create a project in Azure DevOps for Day4 and push the code by running the below commands on VSCode:

git remote add origin $YOURAZUREREPO
git push -u origin all
Note: Make sure to update your Azure repo in the above command

Go to the Azure Portal and Create the Azure App Service by following the instructions in the video

Implement the build pipeline using the classic editor

Understand the use of service connection and service principal

![image](https://github.com/user-attachments/assets/01631c30-e834-460b-8c14-69ff2cea4c74)


Note: You must set the app settings WEBSITE_DYNAMIC_CACHE=0 and WEBSITE_LOCAL_CACHE_OPTION=Never to disable all file caching

Structure of Azure DevOps build Pipeline
![image](https://github.com/user-attachments/assets/ff813306-2826-4927-8831-113b6d742adb)


A trigger tells a Pipeline to run. It could be CI or Scheduled, manual(if not specified), or after another build finishes.
A pipeline is made up of one or more stages. A pipeline can deploy to one or more environments.
A stage organizes jobs in a pipeline, and each stage can have one or more jobs.
Each job runs on one agent, such as Ubuntu, Windows, macOS, etc. A job can also be agentless.
Each agent runs a job that contains one or more steps.
A step can be a task or script and is the smallest building block of a pipeline.
A task is a pre-packaged script that performs an action, such as invoking a REST API or publishing a build artifact.
An artifact is a collection of files or packages published by a run.
![image](https://github.com/user-attachments/assets/f814829b-17b9-4c56-8deb-4aa6e1838a1c)

