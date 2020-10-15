
----------fichier---------------------

syslog-client.yml : playbook concernant les clients syslog (ceux qui envoient leurs logs sur un serveur de log)

syslog-server.yml : playbook concernant les serveurs syslog (ceux qui collectent les logs des clients)

syslog_client.conf : configuration du service "syslog-ng" des clients à envoyer sur les machines clientes

syslog_server.conf : configuration du service "syslog-ng" des serveurs à envoyer sur les machines serveurs

----------étape---------------- 

on lance le déploiement du serveur : ansible-playbook syslog-server.yml

on lance le déploiement des clients : ansible-playbook syslog-client.yml 

-------------vérification----------------- 

sur le serveur de log : cat /var/log/syslog-ng/remote.log
