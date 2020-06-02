# EKS BY Rancher
This repo intends to help customers to create a EKS Cluster managed by Rancher in a EC2 instance.

# Architecture Overview

# Requirements

- AWS Account 

# How to Deploy

## EC2

- Clone this repo: 
` git clone `

- Run Cloudformation on your AWS Account: 

``` 
  cd templates/
  aws cloud formation create stack -- ?? 
```

- Log into EC2 Instance e run the startup script:

```
  cd scripts/
  chmod u+x startup.sh
  ./startup.sh
```

- Check if the Rancher container is running: `sudo docker ps -a`
The output must be something like: 

`ca9ce81a91e8        rancher/rancher:latest   "entrypoint.sh"     2 minutes ago       Up 39 seconds       0.0.0.0:80->80/tcp, 0.0.0.0:443->443/tcp   rancher`








