# blackduckansible

variable are set in /opt/list.yml
```
file_path: /root/downloads/
master1: 93.183.26.164
master2: 93.183.26.165
master3: 93.183.26.166
worker1: 93.183.26.167
worker2: 93.183.26.168
worker3: 93.183.26.169
ha_proxy: 10.131.73.153
etcd_tar_file: etcd-v3.3.9-linux-amd64.tar.gz
etcd_dir: etcd-v3.3.9-linux-amd64
etcd_j2_file: etcd_service.j2
config_j2_file: config.yaml.j2
```

Inside /etc/ansible/hosts
```
[ha_proxy_server]
192.168.0.13
[master_nodes]
esbdslv52.emea.nsn-net.net
esbdsvv51.emea.nsn-net.net
esbdsvv52.emea.nsn-net.net

[worker_nodes]
esbdsvv53.emea.nsn-net.net
esbdsdv51.emea.nsn-net.net
esbdsdv52.emea.nsn-net.net
[master1]
93.183.26.164
[master2]
93.183.26.165
[master3]
93.183.26.166

[worker1]
esbdsvv53.emea.nsn-net.net
[worker2]
esbdsdv51.emea.nsn-net.net
[worker3]
esbdsdv52.emea.nsn-net.net
```
