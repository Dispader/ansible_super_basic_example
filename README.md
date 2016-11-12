# [Super-Basic Ansible](https://youtu.be/xew7CMkL7jY), with Vagrant

## running

First, bring up the vagrant machine.

```Shell
vagrant up
```

Next, execute the example.

```Shell
ansible --inventory-file=hosts dev --module-name=script -a ./script.s
```

NOTE:  If 192.168.33.10 is in your `./.ssh/known_hosts` file, this could be a problem.  I haven't yet found a way to tell Ansible to not use the default known hosts.
