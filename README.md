# Wanderlust-Mega-Project
Jenkins-Mega-Project
# Before Start The Project
1) Create one EC-2 instance on AWS take ssh and Login on command prompt.
2) Create one IAM User and create access key and access id on aws.
3) Install AWSCLI package on ec-2 instance and configure with aws.
 * curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
 * sudo apt-get install unzip -y
 * unzip awscliv2.zip
 * sudo ./aws/install
 * aws configure
 * add access key and access id
4) Install terraform tools package on EC-2 instance.
   * sudo apt-get update && sudo apt-get install -y gnupg software-properties-common
   * wget -O- https://apt.releases.hashicorp.com/gpg | \
gpg --dearmor | \
sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg > /dev/null
   * gpg --no-default-keyring \
--keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \
--fingerprint
  * echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(grep -oP '(?<=UBUNTU_CODENAME=).*' /etc/os-release || lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
  * sudo apt update
  * sudo apt-get install terraform
5) Create ssh-key
  * ssh-keygen
  * Name>>terra-key
6) With the help of terraform tools create EC-2 instance that name is "Master-:wqMachine"
   * terraform init
   * terraform plan
   * terraform apply
7) After That Go To Wanderlust-Mega-Project Direcctory.
8) Now you have to only focus on "Master-Machine"
9) Now you have to all types of tools install in "Master-Machine"
10) Do step-by-step and one-by-one package install on Servers.

## How to take file from EC-2 server to our windows personal machines.
### follow this commad:-
  * scp -i "wardha.pem" ec2-user@98.93.20.149:/home/ec2-user/Wanderlust-Mega-Project/terraform/terra-key .
  *  . means current directory or you can add your path of computer

