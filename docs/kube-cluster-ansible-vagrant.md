bring up an atomic fedora cluster w/ ansible and vagrant:

1. git clone https://github.com/kubernetes/contrib.git
2. export OS_IMAGE=fedoraatomic (regular fedora, regular centos, centos atomic are other options)
3. vagrant up --no-provision --provider=libvirt (virtualbox, openstack and aws are other provider options)
4. [optional, if you want updates] for i in {kube-node-1,kube-master,kube-node-2}; do vagrant ssh $i -c "sudo atomic upgrade"; done && vagrant reload --no-provision
5. vagrant provision kube-master
6. done!

If you don't like vagrant, you can:

1. cd ../
2. cp inventory.example.single_master inventory
3. edit inventory and enter addresses for hosts
4. ./setup

see also: http://www.projectatomic.io/blog/2015/09/clustering-atomic-hosts-with-kubernetes-ansible-and-vagrant/ and https://jebpages.com/2016/02/05/testing-flannel/
