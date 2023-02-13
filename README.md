# aws-vm-scheduler


## Build docker image

docker build -t awsvmscheduler:v1.0 . 

## Run docker image. 

Note:  Need to export the AWS parms before you run it. 

docker run -e AWS_DEFAULT_REGION=us-east-1 -e AWS_SECRET_ACCESS_KEY=$AWS_SECRET_ACCESS_KEY -e AWS_ACCESS_KEY_ID=$AWS_ACCESS_KEY_ID -e ec2_command="start" -e ec2_instanceIds="i-00db611adab6f713d,i-0ef1d87bdf4dd3ad1" -it awsvmscheduler:v1.0 


## sample docker files 

Dockerfile*