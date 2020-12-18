Script tonto que lanza un script de powershell en el servidor hyperv 2

Como se lanza desde el servidor **ansible**
```
ansible-playbook main.yml
git add . && git commit -am 'Crear equipo en Hyper-V.... 1' && git push
```
Se ha de anadir al fichero: vim /etc/ansible/hosts
```
[hyper-v]
host2.ilba.cat

[hyper-v:vars]
ansible_ssh_user=administrator@ILBA.CAT
ansible_ssh_pass=password_del_dominio
ansible_ssh_port=5985
ansible_connection=winrm
```

