# Comandos para conexiones SSH exitosas

### Para generar una llave nueva
```
ssh-keygen -t rsa -b 4096 -C "nombre@tudominio.com" -f ~/.ssh/millavefavorita
```

### Darle permisos de acceso a tu llave
```
chmod 600 ~/.ssh/millavefavorita
```

## Como servidor para aceptar conexiones entrantes
Actualiza los paquetes

`
sudo apt update
`

Instala el servidor openssh

`sudo apt install -y openssh-server`

Comprueba que el servidor OpenSSH está funcionando

`sudo systemctl status ssh`


### Inicia el SSH agent en segundo plano y agregale tu llave privada
```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/intertech_rsa
```
