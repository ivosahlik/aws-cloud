## EC2 - Elastic Computing CLoud

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
chmod 400 ivosahlik-dev-eu-central-1-key.pem
ssh -i ivosahlik-dev-eu-central-1-key.pem ec2-user@3.120.16.116
