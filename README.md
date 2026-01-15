https://roadmap.sh/projects/simple-monitoring-dashboard
# Simple-monitoring

Installation et configuration
 git clone https://github.com/snsuzie/Simple-monitoring.git
 je me positionne sur le disue D en faisant cd d: puis
cd  Roadmapsh_Project/Simple-monitoring "pour cloner le rep depot github"

Rendre le script exécutable et lancer l’installation : chmod +x setup.sh
./setup.sh

Une fois l’installation terminée, accéder au dashboard Netdata : http://localhost:19999
# Monitoring du système

Netdata surveille automatiquement les métriques suivantes :
Utilisation du CPU (globale et par cœur)
Mémoire RAM et swap
Entrées / sorties disque (Disk I/O)
Load average
Trafic réseau
Toutes les métriques sont affichées en temps réel dans le dashboard web.

Le fichier d'alerte : /etc/netdata/health.d/cpu_usage.conf à modifier en fonction de ce qu'on veut de netdata

Pour tester notre monitoring : chmod +x test_dashboard.sh
./test_dashboard.sh

Il Génère une charge CPU artificielle, Effectue des opérations de lecture/écriture disque et Déclenche les alertes Netdata.

Nettoyer le système et supprimer Netdata : chmod +x cleanup.sh
./cleanup.sh

