# SAWI

### Simple Aws Web Interface

This is a Flask app that lets you deploy, edit and delete static S3 websites and Virtual Machines to your AWS account.


## Installation

It makes use of Pulumi, so you will need it installed for it to work you can learn more at: https://www.pulumi.com/docs/get-started/install/

You will also need an AWS account and the CLI installed: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html 

And configured: 

`aws configure`

Once you got this covered run: 

`pulumi new`

This command will prompt you for login details, so you will have to create a Pulumi account in case you dont have one, and select a template, I used aws-python in this case. 

Now you are ready to go! All you need is to clone the repo and store the files locally inside the pulumi project you just created.

## Running the app

To get the app up and running locally all you have to do is activate the venv and then execute: 

`flask run`

Theres an enviroment variable named **PULUMI_ORG** that has to be passed when running the script and it has to be equal to your Pulumi username for the App to work properly otherwise it will give you a 404 error when trying to open the website.

## VMs and you

When you create a VM using the app you will ask you to introduce a public ssh key.
If you don´t know how to do this please visit: 

https://www.ssh.com/academy/ssh/public-key-authentication

for more information about this.




