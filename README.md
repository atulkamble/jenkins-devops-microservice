# jenkins-devops-microservice

### Pre Code
```
echo "# jenkins-devops-microservice" >> README.md\ngit init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/atulkamble/jenkins-devops-microservice.git
git push -u origin main
```
### After Code
```
git add .
git commit -m "code"
git push origin main
```
### Project Settings are as follows

### System Configurations >> System 
```
myMaven
myDocker
```

### Within Code 
```
>> Dockerfile >> docker build >> Replace your dockerhub username
```

### Steps
```
Create Pipeline >> jenkins-devops-microservice-pipeline

Description >> jenkins-devops-microservice

(Optional) Build Triggers >> Build periodically

Poll SCM >> Schedule >> * * * * *

Pipeline >> Definition >> Pipeline Script from SCM 
SCM >> git 
Repository URL >> https://github.com/atulkamble/jenkins-devops-microservice
Credentials >> atulkamble/******
Branches to build >> Branch Specifier (blank for 'any') >> main
Script path >> Jenkinsfile

>> SAVE
```
