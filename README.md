# Amazon ECS PHP Simple Demo App

# Build Docker images
docker build -t dieple/docker-ec2-php-app .

# Run the docker image
docker run -p 80:80 dieple/docker-ec2-php-app

# To run on AWS instances
1) Login to aws instances
2) git clone https://github.com/dieple/docker-ec2-php-app.git
3) Register the task definition simple-app-task-def.json with this command: 
aws ecs register-task-definition --cli-input-json file://simple-app-task-def.json
4) Run the console-sample-app task definition
aws ecs run-task --task-definition console-sample-app
