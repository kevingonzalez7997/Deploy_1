<h2>Setting Up GitHub</h2>
First create a new repo this is where we will upload the app/This will be our staging environment
<br><br>
Upload the app files to the new repo
<br><br>
Make sure you get your token from GitHub for the repo that you have created (Jenkins will need this later)
<h2>IAM</h2>
Before you can test the code in Jenkins make sure you set up the correct IAM Permissions
<br><br>
you need  2 roles, one for Beanstalk and one for the EC2
<br><br>
add AWSElasticBeanstalkWebTier,workerTier,MulticontainerDocker as the permissions
<br><br>
This has to be done before you run it bc it will control who has access to what
<h2>Jenkins</h2>
login to Jenkins
<br><br>
Create a new item
<br><br>
Link the new repo using the token created earlier
<br><br>
If test runs are successful you can run in AWS
<h2>AWS</h2>
Create an application to start!!
<br><br>
Give it a name
<br><br>
pick the platform (python 3.9)
<br><br>
upload the zipped file (from the new repo) make sure you zip without the parent folder!
<br><br>
select ElasticEC2 
<br><br>
pick default vpc
<br><br>
select az
<br><br>
Lastly, you have to finish setting up some settings for your EC2 instance such as root volume type and size
<br><br>
While the EC2 instance is pending the running state, it is important not to forget to close your eyes and pray to increase the launch probability! 


![Screenshot 2023-08-15 210425](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/a4254e30-468e-44af-be62-f1d79e39c58c)
<br>
![Deployment_1_Kevin_G](https://github.com/kevingonzalez7997/Deploy_1/assets/59447523/63c46025-d6f6-42df-aeb6-fa00f2554699)
