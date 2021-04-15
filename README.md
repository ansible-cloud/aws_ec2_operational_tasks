# AWS EC2 Operational Tasks

This Ansible Project showcase multiple AWS (Amazon Web Services) operational tasks fully automated with Ansible Playbooks.

An operational tasks is a routine task an operator (cloud administer) has to do outside of provisioning and deprovisioning resources.  Declarative automation (such as AWS CloudFormation templates) are great until someone manually, or some tool outside of CloudFormation starts interacting with the public cloud.  There is always use cases for imperative repeatable tasks that operators are doing manually.

# Glossary of AWS terms

**ec2** - Amazon Elastic Compute Cloud, Secure, resizable compute capacity in the cloud.

**ec2 region** - Amazon cloud computing resources are hosted in multiple locations world-wide. These locations are composed of AWS Regions, Availability Zones, and Local Zones. Each AWS Region is a separate geographic area. Each AWS Region has multiple, isolated locations known as Availability Zones. [read more here](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html)

**ec2 instance** - Any compute deployment within the Amazon EC2 service.



# Playbook Examples

## Retrieve and Stop

`playbooks/stop_instances.yaml`


```yaml
ansible-playbook stop_instances.yaml -e "your_region=us-west-1"
```

This Ansible Playbook will retrieve all instances from the specified region `us-west-1` and stop them.
