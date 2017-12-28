使用方法
```
$ ansible-playbook -i inventory vpc.yml -e 'acname=launch' --tags launch
$ ansible-playbook -i inventory vpc.yml -e 'acname=terminate' --tags terminate
```

尴尬的是 vpc 删除总不成功，无法删除主路由表，也无法删除 default 路由表。