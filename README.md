# ookla_speedtest_install_Arole
ansible role to install ookla speedtest   

# prerequisitesyum  install      
yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -y   
yum install ansible -y   
yum install git vim wget unzip   
   
useradd ansible   
echo 'apnansible2020!' | passwd --stdin ansible   
echo "ansible ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/ansible   
su - ansible   
(ansible)$ssh-keygen   
(ansible)$ssh-copy-id localhost   
(ansible)$exit   
(root)$ssh-keygen   
(root)$ssh-copy-id localhost   
   
# usage   
ansible-playbook ookla.yml -i inventory 
