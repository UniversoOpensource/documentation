# Documentação 

Este repositorio tem como obejtivo registrar comandos, dicas e informações usados no meu dia a dia.

## Dicas (especificos):

### Cryptsetup

Consultar slot usados
```
cryptsetup luksDump /dev/sdX1 | grep Slot
```

Adicionar novo slot
```
cryptsetup luksAddKey /dev/sdX1
```


### DOCKER 

### GIT

Comparar dois commit's 
```
git diff XYZ ZYX > Arquivo-Saida-Do-Log
```

### LINUX

Montar partição remota via ssh 
```
sshfs -o allow_other root@172.16.0.1:/media/hd/oldFiles /media/servidor
```

### Screen 

### Ubuntu

Adicionando novo usuario (admin) no ubuntu
```
sudo adduser user 
sudo usermod -aG sudo user
```
Desativar mensagens de erro do ubuntu 
```
sudo sed -ie 's/enabled=1/enabled=0/g' /etc/default/apport
```

### Virtualbox

#### Trabalhando com virtualbox em linah de comando

Add extpack 
```
VBoxManage extpack install Oracle_VM_VirtualBox_Extension_Pack-__VERSAO__.vbox-extpack
```

Export imagem
```
vboxmanage list vms
vboxmanage export nome_vm -o /loca/nome_da_imagem.ova
```


## Dicas (Outros):

### Dicas multimidia

#### Gravar CDROM/DVD via linha de comando

```
sudo growisofs -dvd-compat -speed=8 -Z /dev/cdrom=/tmp/imagem.iso
```

## Tabela de repositorios:
