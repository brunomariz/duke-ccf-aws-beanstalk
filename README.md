# Duke - Cloud Computing Foundations - AWS Beanstalk

Demo repo for AWS Beanstalk assignment of Cloud Computing Foundations course.

AWS Beanstalk CLI allows you to deploy applications without having to take care of setting up infrastructure such as load balancers, compute instances, security groups, etc.

## Steps to create AWS Beansalk applicaion

1. Open Cloud9
2. Install EB CLI - https://github.com/aws/aws-elastic-beanstalk-cli-setup
3. Create venv and activate it
4. Install Flask
```
pip install flask
```
6. Create requirements.txt
```
pip freeze > requirements.txt
```
7. Create applicaion.py - https://github.com/noahgift/Flask-Elastic-Beanstalk/blob/main/application.py
8. Test locally
9. Create .ebignore
10. Create new environment

Create app
```
eb init -p python-3.8 flask-cloud-data
```

Create Role - https://stackoverflow.com/questions/30790666/error-with-not-existing-instance-profile-while-trying-to-get-a-django-project-ru

Create the environment
```
eb create flask-cloud-data-env
```
11. Open AWN Beanstalk Environments (make sure you select the correct region where the environment was created)
12. Click the domain link to test it out
13. Terminate the environment
```
eb terminate flask-cloud-data-env
```
14. Check it really was deleted on AWS Beanstalk Environments
![image](https://github.com/brunomariz/duke-ccf-aws-beanstalk/assets/48870924/f3527680-74bc-42bf-8bdc-8e941dab2414)
