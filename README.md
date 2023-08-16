First, create a new repo this is where we will upload the app/This will be our staging environment

Upload the app to new repo

Make sure you get your token from GitHub for the repo that you have created

-------------------------------------------------------------------------------------------------------------------------------

Before you can test the code in Jenkins make sure you set up the correct IAM Permissions
This has to be done before you run it as it will control who has access to what

once you have the token and you set up the role you can go ahead and go to Jenkin and create a pipeline to deploy and test the application

If everything is working without any errors we can move on to launching the app manually

-------------------------------------------------------------------------------------------------------------------------------

Create an application to start!!

Give it a name

pick the platform platform-python(3.9)

upload zipped file ( of new repo app) make sure you zip without the parent folder!

pick ElasticEC2 

pick default vpc

select az

Lastly, you have to finish setting up some settings for your EC2 instance such as root volume type and size

-------------------------------------------------------------------------------------------------------------------------------

While the EC2 instance is running it is important not to forget to close your eyes and pray to increase the launch probability! 


![Screenshot 2023-08-15 210425](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/a4254e30-468e-44af-be62-f1d79e39c58c)


![Deployment_1_Kevin_G](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/63c46025-d6f6-42df-aeb6-fa00f2554699)
