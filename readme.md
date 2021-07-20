aws ecr get-login-password --region ap-south-1 | sudo docker login --username AWS --password-stdin 589117662781.dkr.ecr.ap-south-1.amazonaws.com

sudo docker build -t jquery1-eks:latest 589117662781.dkr.ecr.ap-south-1.amazonaws.com/jquery1-eks:$BUILD_NUMBER

sudo docker push 589117662781.dkr.ecr.ap-south-1.amazonaws.com/jquery1-eks:$BUILD_NUMBER

lokesh