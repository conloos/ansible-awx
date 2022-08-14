# Ansible role for building and running awx.

**summary**
This role is for building and running ansible. 
Look in the tasks directory for each configuration.
All configurations are held atomically via their own files. 

## Variables that have to be defined

| variable | description |
| -------- | ----------- |
| version_tags.awx | Version to build |
| pg_password | Postgres Admin password |
| broadcast_websocket_secret | broadcast_websocket_secret |
| secret_key | secred_key |
| admin_password | administrator account (admin) password |
| ssl_crt_path | path to crt-file for the nginx, default: </etc/ssl/FQDN.key> |
| ssl_key_path | path to key-file for the nginx, default: </etc/ssl/FQDN.key> |