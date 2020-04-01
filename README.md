# ldap-server-mock
Mock ldap server for tests

## Run
```bash
docker run -d -p 3004:3004 thoteam/ldap-server-mock
```

## Overriding default config and users
```bash
docker run -d \
-v <path-to-conf>:/srv/ldap-server-mock-conf.json \
-v <path-to-userdb>:/srv/ldap-server-mock-users.json \
-p 3004:3004 thoteam/ldap-server-mock
```
