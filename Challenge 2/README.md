# Challenge 2

## What it does
- Query the metadata of an ec2 instance within AWS and provide a json formatted output. 
- Retrieve the value of a particular data key.

## How to install
- Spin an EC2 Linux instance on AWS
- SSH into the instance
- Install Python 3 and git on your instance 
    - `sudo yum install python3 git`
- Clone the repository
  - `git clone https://github.com/bluprince13/aws-metadata-json`
- Install pipenv
  - `sudo pip3 install pipenv`
- Open the repository on your instance
  - `cd aws-metadata-json`
- Install project dependancies
  - `pipenv install`


## How to run
- Open the `src` folder
  - `cd aws-metadata-json/src`
- Run script you need:
  - `python3 get_instance_metadata.py`
  - `python3 get_key.py`

## How it works
- It makes use of the http://169.254.169.254/latest/meta-data link-local address. Instance metatada is provided at this link, but only when you visit it from a running instance.