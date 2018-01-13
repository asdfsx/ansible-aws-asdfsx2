使用方法
```
$ ansible-playbook -i contrib/ec2.py kerberos.yml -e 'acname=install' --tags install
```

测试kerberos
```
# 列出Kerberos中的所有认证用户，即principals
kadmin.local -q "list_principals"
# 添加认证用户，需要输入密码
kadmin.local -q "addprinc user1"
# 使用该用户登录，获取身份认证，需要输入密码
kinit user1
# 查看当前用户的认证信息ticket
klist
# 更新ticket
kinit -R
# 销毁当前的ticket
kdestroy
# 删除认证用户
kadmin.local -q "delprinc user1"
```