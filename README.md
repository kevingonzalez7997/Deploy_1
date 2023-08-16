First make sure you get your token from GitHub from the repo that you have forked

once you have the token you can go ahead and go to Jenkin and create a pipeline to deploy and test the application

once I had it running I was able to go to AWS and create my own ec2 instance

I give it a name

pick my platform-python(3.9)

upload my zipped file ( of my app) make sure you zip without the parent folder

pick ElasticEC2 

pick default vpc

select az

after selecting the instance and scaling the ec2 should be ready to launch !!

