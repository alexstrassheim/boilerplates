# Missing Indices

Anmelden mit dem Nutzer `www-data` am `nextcloud` Docker-Container und folgenden Befehl ausführen: 

```bash
su -s /bin/bash www-data -c 'php occ integrity:check-core'
```

```bash
su -s /bin/bash www-data -c 'php occ db:add-missing-indices' 
```

```bash
su -s /bin/bash www-data -c 'php occ maintenance:repair --include-expensive' 
```

```bash
# OIDC provider the default login method
su -s /bin/bash www-data -c 'php occ config:app:set --value=0 user_oidc allow_multiple_user_backends'
