

----------fichier---------------------

servers-client.yml : playbook concernant tous les serveurs 

syslog-server.yml : playbook concernant les serveurs syslog (ceux qui collectent les logs des clients)

syslog_client.conf : configuration du service "syslog-ng" des clients à envoyer sur les machines clientes

syslog_server.conf : configuration du service "syslog-ng" des serveurs à envoyer sur les machines serveurs

----------étape----------------

on lance le déploiement du serveur : ansible-playbook syslog-server.yml

on lance le déploiement des clients : ansible-playbook servers-client.yml

