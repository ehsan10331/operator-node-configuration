# operator-node-configuration
    1  sudo yum update -y
    2  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
    3  unzip awscliv2.zip
    4  sudo ./aws/install
    5  aws --version
    6  aws configure
    7  aws sts get-caller-identity
    8  sudo yum update -y
    9  curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.22.15/2023-03-16/bin/linux/amd64/kubectl
   10  chmod +x ./kubectl
   11  sudo mv ./kubectl /usr/local/bin
   12  kubectl version --client
   13  kubectl version
   14  file /usr/local/bin/kubectl
   15  sudo rm /usr/local/bin/kubectl
   16  curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   17  chmod +x kubectl
   18  sudo mv kubectl /usr/local/bin/
   19  kubectl version --client
   20  curl -LO "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_$(uname -s)_amd64.tar.gz"
   21  tar -xzf eksctl_$(uname -s)_amd64.tar.gz
   22  sudo mv eksctl /usr/local/bin
   23  eksctl version
   24  eksctl create cluster --name eks-demo --region us-east-1 --nodegroup-name worker-node --node-type t3.medium --nodes 2 --nodes-          min 1 --nodes-max 4
   25  kubectl get all
   26  history
