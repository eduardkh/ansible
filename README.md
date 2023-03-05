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
# passlib for password encryption
sudo pip install passlib

# create ansible-vault file
ansible-vault create 'create user vault/secret.yaml'

# example user in secret.yaml file
username: david
pwhash: password

# edit ansible-vault file
ansible-vault edit 'create user vault/secret.yaml'

# Run playbook
ansible-playbook --ask-vault-pass 'create user vault/playbook.yaml'
```
