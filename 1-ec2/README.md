## EC2 - Elastic Computing Cloud - Step By Step

## Recommended name tag structure
```
<project>-<service>-<env>-<region>-<type>-<index>
ivosahlik-app1-dev-eu-central-1-api-01
```

## Recommended key pair name structure
```
<project>-<env>-<region>-key
ivosahlik-dev-eu-central-1-key -> ivosahlik-dev-eu-central-1-key.pem
```

## Recommended security group name structure
```
<project>-<service>-<env>-sg
ivosahlik-app1-eu-central-1-sg
```

## EC2 - SSH From Local
```
chmod 400 ivosahlik-dev-eu-central-1-key.pem
```

## Public IPv4 address - Connect from localhost to ec2
```
ssh -i ivosahlik-dev-eu-central-1-key.pem ec2-user@18.185.83.221
```

## Docker
```
sudo yum install docker
sudo docker version
sudo systemctl start docker.service
sudo systemctl stop docker.service

sudo docker run hello-world
```

## Nginx
Set inbound rules, add type http -> Welcome to nginx!
```
sudo docker run -p 80:80 nginx
```