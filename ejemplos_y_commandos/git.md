# Ejemplis de GIT

Simply use chown to change the ownership of the files to your current user, for instance:
```
chown -R $(whoami) .
```

eval "$(ssh-agent -s)"
ssh-add ~/.ssh/from_develop_inter

cd /bench/apps/frappe-app
git remote add origin git@github.com:Interconectando/eac_interconectando.git
git branch -M dev-version-14
git push -u origin dev-version-14 --force
