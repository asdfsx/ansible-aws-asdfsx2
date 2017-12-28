使用方法
```
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=keypair' --tags keypair
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=launch' --tags launch
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=ssh' --tags ssh
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=optimize' --tags optimize
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=start' --tags start
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=stop' --tags stop
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=terminate' --tags terminate
$ ansible-playbook -i contrib/ec2.py ec2.yml -e 'acname=describe' --tags describe
```