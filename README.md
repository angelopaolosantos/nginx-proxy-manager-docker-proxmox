# nginx-proxy-manager-proxmox

terraform init --backend-config=config.pg.tfbackend 

# Install Terraform Collection for Ansible
ansible-galaxy collection install cloud.terraform

# Print Terraform Inventory
ansible-inventory -i ./ansible/inventory.yaml --graph --vars

# Run Ansible Playbook
ansible-playbook -i ./ansible/inventory.yaml ./ansible/playbook.yaml

export ANSIBLE_HOST_KEY_CHECKING=False

ssh -o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no -i .ssh/my-private-key.pem root@192.168.254.213

terraform state pull > terraform.tfstate

terraform show -json

### Default Administrator User
Email:    admin@example.com
Password: changeme

https://github.com/elasticdog/transcrypt