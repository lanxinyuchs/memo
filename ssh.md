允许root登录:
vim /etc/ssh/sshd_config
修改PermitRootLogin yes
重启服务 service ssh restart

ssh免密登录：
ssh-keygen -t rsa -N '' -q -f ~/.ssh/id_rsa
scp ~/.ssh/id_rsa.pub root@10.240.179.102:/root/.ssh/authorized_keys
