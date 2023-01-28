# Ansible role for building and running awx.

**summary**
This role is for building and running ansible. 
Look in the tasks directory for each configuration.
All configurations are held atomically via their own files. 

## Variables that have to be defined

| variable | description |
| -------- | ----------- |
| cloudinit_fqdn | f
| version_tags.awx | Version to build |
| pg_password | Postgres Admin password |
| broadcast_websocket_secret | broadcast_websocket_secret |
| secret_key | secred_key |
| awx_install_path | Path to install the sources. |
| admin_password | administrator account (admin) password |
| awx_ssl_crt_path | path to crt-file for the nginx, default: **</etc/ssl/awx@FQDN.key>** |
| awx_ssl_key_path | path to key-file for the nginx, default: **</etc/ssl/awx@FQDN.key>** |
| path_to_step_cli | Path to the step-ca executables. |

## Supported Tags

| Tag | description |
| --- | ----------- |
| install_tools | Install Packages |
| create_certificates | Install ACME Certs |

