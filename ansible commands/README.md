Ansible installation:
after coonecting to instance --> check for python --> if python is not installed; yum install python-pip --> pip install ansible

working with ansible:-
ansible all -m ping
ansible all -m ping -i hosts
ansible all -m command -a "date" -i hosts
ansible all -m yum -a "name=git" -i hosts -b [here, instead of all we can give the partricular instance name ; in name we have to give what we want to install; -b is since we are not in root we are telling BECOME root]
