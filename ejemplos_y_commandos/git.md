# Ejemplis de GIT

Simply use chown to change the ownership of the files to your current user, for instance:
```
chown -R $(whoami) .
```
```
eval "$(ssh-agent -s)" 
ssh-add ~/.ssh/from_develop_inter 

cd /bench/apps/frappe-app 
git remote add origin git@github.com:Interconectando/eac_interconectando.git 
git branch -M dev-version-14 
git push -u origin dev-version-14 --force 
```

## Crea llave en tu servidor
```
ssh-keygen -t rsa -b 2048 -C "mi_correo@gmail.com" -f ~/.ssh/mi_llave 
chmod 600 ~/.ssh/mi_llave
cat ~/.ssh/mi_llave.pub
```

## Descarga app
```
eval "$(ssh-agent -s)" 
ssh-add ~/.ssh/mi_llave
``` 
#### Instala la app de INTERCONECTANDO® AVC SERVER
```
cd /opt/avc-server/bench

bench get-app git@github.com:Interconectando/interconectando_avc_server.git --branch version-14
	Pregunta
	Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
```

#### Instala la app de INTERCONECTANDO® AVC SERVER
```
bench --site interval.intercam.com.mx install-app interconectando_avc_server
```
