# Amazon ECS PHP Simple Demo App

# Build Docker images
docker build -t dieple/docker-ec2-php-app .

# Run the docker image
docker run -p 80:80 dieple/docker-ec2-php-app
