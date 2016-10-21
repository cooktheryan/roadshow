# To Launch

ansible-playbook -e 'region=us-east-1 public_hosted_zone=rcook-aws.sysdeseng.com keypair=OSE-key' playbooks/infrastructure.yaml

# To Teardown

ansible-playbook -e 'region=us-east-1 public_hosted_zone=rcook-aws.sysdeseng.com keypair=OSE-key ci=false' playbooks/teardown.yaml

Note: When ci=true all EBS volumes in an account will be removed. Used with caution.
