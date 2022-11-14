# CentOS infra-scripts

Scripts used for ad-hoc/one-shot tasks in CentOS Infra
Organized in folders by type of scripts

## Koji/cbs
 * cbs-infra-promote: quickly "promote" pending pkgs from one tag to another (like `candidate` => `testing` => `release `

## Pagure
 * pagure-create-repo: just using pagure api token and curl to quickly create a project in a particular namespace

## Opennebula
 * os-to-one: quickly export from openstack (as snapshot) an instance and import it opennebula

## Ansible
 * convert-ansible-tasks-to-fqcn: simple bash script to convert existing .yml tasks files to FQCN through mapping 

## AWS
 * upload-ami-image: takes a built .raw cloud image, upload to S3 bucket as snapshot, make an AMI and test deploying it
 * sync-ami-to-regions: asks for previously tested AMI ID, and make it public and sync to 20 AWS regions also producing needed output for www.centos.org/ and wiki content
