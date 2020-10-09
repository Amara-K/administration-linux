Action à réaliser avant utilisation : 
-modifier adresse ip client/server dans fichier "hosts"

-modifier adresse ip du server log dans fichier "syslog_client.conf"


fichier:
syslog-client.yml : playbook concernant les clients syslog (ceux qui envoient leurs logs sur un serveur de log)

syslog-server.yml : playbook concernant les serveurs syslog (ceux qui collectent les logs des clients)

syslog_client.conf : configuration du service "syslog-ng" des clients à envoyer sur les machines clientes

syslog_server.conf : configuration du service "syslog-ng" des serveurs à envoyer sur les machines serveurs
