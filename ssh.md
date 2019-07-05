ssh-keygen -t rsa -N '' -q -f ~/.ssh/id_rsa
scp ~/.ssh/id_rsa.pub root@10.240.179.102:/root/.ssh/authorized_keys
