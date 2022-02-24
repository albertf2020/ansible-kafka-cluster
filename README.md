# Kafka Ubuntu 18.04 virtual cluster

Easily create a local Kafka cluster with Zookeeper quorum via Vagrant + Ansible. Or just use the Ansible playbooks.

## Usage

Depending on your hardware and network connection, the script execution might take between 10-20 minutes.

### Start the cluster with Vagrant

```
vagrant up or if you modified anything in site.yml/Vagrantfile and etc. use vagrant up --provision 2>&1 | tee java_log.txt
```

```
vagrant ssh zk-node-{1,2,3}
```

```
vagrant ssh kafka-node-{1,2,3}
```

### Suspend a Kafka node

From  your host, take down a Kafka node

```
vagrant suspend kafka-node-3
```


