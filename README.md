# Pupici
Pupici: Home Automation System

## Backup
Each container has access to a volume that points to a directory on the host system. Then [ofelia](https://github.com/mcuadros/ofelia) executes the different backup commands directly in the containers. Use NFS share on the host so that backups are safely stored on a remote server.
## Tools
### Define alias to connect to openhab shell from linux (debian) host
- Create alias in .bash_aliases
```sh
alias oh="docker exec -it openhab /openhab/runtime/bin/client -p habopen"
alias oh_shell="docker exec -it openhab bash"
```