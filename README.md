# ansible

> basic information [Ansible: From Basics to Guru](https://github.com/sandervanvugt/ansiblecvc)

```bash
basic config in 'ansible.cfg'
basic inventory in 'inventory'
```

> adhoc ping

```bash
# all hosts
ansible -m ansible.builtin.ping all
# rocky hosts
ansible -m ansible.builtin.ping rocky
# ubuntu hosts
ansible -m ansible.builtin.ping ubuntu
```

> ansible-playbook ping

```bash
ansible-playbook ping/playbook.yaml
```

> create user vault

```bash
sudo pip install passlib
ansible-playbook --ask-vault-pass create\ user\ vault/playbook.yaml
```
