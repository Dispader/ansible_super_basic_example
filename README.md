# [Super-Basic Ansible](https://youtu.be/xew7CMkL7jY), with Vagrant

## running

First, bring up the vagrant machine.

```Shell
vagrant up
```

Next, execute the example.

```Shell
ansible --private-key=.vagrant/machines/default/virtualbox/private_key --user vagrant --inventory-file=hosts dev -m script -a ./script.sh
```

NOTE:  If 192.168.33.10 is in your `./.ssh/known_hosts` file, this could be a problem.  I haven't yet found a way to tell Ansible to not use the default known hosts.
