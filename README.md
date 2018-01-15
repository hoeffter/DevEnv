# DevEnv
Ansible Files to bootstrap my development environment

1. Add User

```useradd -m USERNAME```
  
2. Add User to sudoers file
  
```sudo adduser USERNAME sudo```

3. change user to don't need password for sudo

```
sudo vim /etc/sudoers
USERNAME ALL=(ALL) NOPASSWD: ALL
```

4. Install Ansible
  
http://docs.ansible.com/ansible/latest/intro_installation.html#latest-releases-via-apt-ubuntu

```
$ sudo apt-get update
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible
```

5. Clone Repo

```
git clone https://github.com/hoeffter/DevEnv.git
```

6. Change Variables

Mainly in Playbook.yml
