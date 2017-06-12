# vagrant_splunk_cluster
Vagrant config for creating a Splunk single site indexer and SHC

Install prerequisites:
  - VirtualBox installed
  - Vagrant installed
    - vagrant plugin install vagrant-vbguest

This will create the following VMs:
  - 192.168.30.105		ansiblemaster
  - 192.168.30.106		splunkidx01
  - 192.168.30.107		splunkidx02
  - 192.168.30.108		splunkidx03
  - 192.168.30.109		splunkshc01
  - 192.168.30.110		splunkshc02
  - 192.168.30.111		splunkshc03
  - 192.168.30.112		splunkcm01
  - 192.168.30.113		splunkuf01
  - 192.168.30.114		splunkuf02

Todo:
  - Once splunk_cluster repo is made public add final config to this project to automate the pull.
  - Set cron job to run Ansible splunk build
