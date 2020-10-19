# Scenario

Imagine you’re company is writing a cool new website. The developers are going to be adding features to the website. To help them speed their releases to Production, you also want to template and automate building an EC2 server. You do this by creating configuration formulas that your servers can use to automatically install the needed software to run Python and Flask, and pull the latest Flask application repo to the server.
First, create the Flask app. There’s a QuickStart Guide to working with [Flask](http://flask.pocoo.org/docs/quickstart/). Just follow the directions, displaying “hello world” is fine.

While the developers are writing code, you want to allow them to deploy code themselves using any of these (or combination): Ansible/Terraform. They should be able to deploy the blog app remotely using a combination automation tools and/or command line tools (bash + aws cli).
Here are the specs you need:

- **OS**: Ubuntu Server 18.04 64-bit
- **App Server**: Gunicorn/Nginx
- **Python**: 3.8
- **Flask**: 1.1.x

In developing both the app and automation, use GitHub and try to keep a decent history of how you approached the project.

Deliverables

1. A GitHub repo to the Flask app.
2. A GitHub repo to the automation.
3. Script/Tools that will:
    - Launch the EC2 server using an AMI. (or using docker , see bonus section)
    - Begin the configuration management / bootstrapping of the server using your automation tool of choice.
    - Deploy the app
4. Access to the AWS Account you create.

**DO NOT CHECK THIS INTO GITHUB WITH AWS KEYS**

Remember to use security groups to restrict port access.

Leave detailed instructions on how instantiate and access the web app.

**Bonus Section**

* Terraform w/Remote State
* Build and run a docker container
