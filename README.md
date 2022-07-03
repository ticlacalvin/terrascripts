# terrascripts
Our goal in this project is to write a srcipt which will create infrastructures with Terraform: one Control pane and two worker nodes. Once terraform has provionned 
automatically the infrastructures, Ansible will take over and set up a k8s cluster, configure the servers and deploy the applications using some playbooks with dynamic inventory.
We are using Redhat in the Infra_config server and Ubuntu for the three servers inside the cluster.
To initialize Terraform, create a direcctory called terraform_scripts and put together main.tf, security-group.tf and variables.tf then run terraform init in that directory.
