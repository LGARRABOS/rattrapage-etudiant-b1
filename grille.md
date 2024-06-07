Voici une grille de notation sur 20 pour le sujet de réseau, avec chaque emoji représentant une question ou un attendu. La notation est répartie de manière à couvrir chaque aspect du TP de manière équilibrée :

### Grille de Notation

#### Partie 1 : Setup du patron (4 points)
1. 🌞 Créez une VM avec VirtualBox, nommée ```Patron``` (0.5 point)
   - VM créée et nommée correctement : 0.5 point
2. 🌞 Configurez la VM avec 2 interfaces réseaux. La première en NAT et la deuxième en Host-Only. (0.5 point)
   - Interfaces réseau configurées correctement : 0.5 point
3. 🌞 Installez Rocky Linux minimal sur la VM. (1 point)
   - Rocky Linux minimal installé correctement : 1 point
4. 🌞 Définissez une IP statique à la VM. (0.5 point)
   - IP statique configurée : 0.5 point
5. 🌞 Donnez un hostname à la machine. (0.5 point)
   - Hostname défini correctement : 0.5 point
6. 🌞 Configurez SSH pour administrer la machine (avec échange de clés). (1 point)
   - SSH configuré avec échange de clés : 1 point

#### Partie 2 : Premier test réseau (4 points)
1. 🌞 Configurez correctement ces 2 VM. (2 points)
   - Hostname défini sur chaque machine : 0.5 point
   - Configuration réseau correcte (fichiers de configuration réseau) : 1 point
   - Configuration des fichiers hostname correcte : 0.5 point
2. 🌞 Testez la connectivité entre les deux machines avec un ping. (2 points)
   - Ping entre `etudiant` et `mentor` réussi : 2 points

#### Partie 3 : Un petit peu de routage (6 points)
1. 🌞 Configurez correctement ces 3 VM. (2 points)
   - Configuration correcte des interfaces réseau pour `routeur`, `mentor` et `etudiant` : 2 points
2. 🌞 Configurez le routeur pour qu'il puisse faire le lien entre les deux réseaux. (2 points)
   - Routeur configuré correctement pour relier les deux réseaux : 2 points
3. 🌞 Testez la connectivité entre les machines : (2 points)
   - `etudiant` et `routeur` : 0.5 point
   - `mentor` et `routeur` : 0.5 point
   - `etudiant` et `mentor` : 1 point
4. 🦈 Faites des captures avec WireShark pour prouver que les machines communiquent bien entre elles. (2 points)
   - Captures WireShark fournies et correctes : 2 points
5. 🌞 Donnez à `etudiant` et `mentor` un accès à internet via le routeur. (2 points)
   - Accès internet configuré et fonctionnel pour `etudiant` et `mentor` : 2 points

#### Partie 4 : Web (3 points)
1. 🌞 Installez un serveur web Apache sur la machine `mentor`. (0.5 point)
   - Apache installé correctement : 0.5 point
2. 🌞 Créez un fichier HTML qui va afficher le nom de la machine (à vous de trouver où le mettre). (0.5 point)
   - Fichier HTML créé et affichant le nom de la machine : 0.5 point
3. 🌞 Créez un nouvel utilisateur nommé `apache` qui va gérer le serveur web (donnez-lui les accès aux dossiers/fichiers dont il a besoin). (0.5 point)
   - Utilisateur `apache` créé et configuré correctement : 0.5 point
4. 🌞 Ouvrez le port firewall. (0.5 point)
   - Port firewall ouvert : 0.5 point
5. 🌞 Testez l'accès au serveur web depuis la machine `mentor` à l'aide d'une commande curl. (0.5 point)
   - Accès au serveur web depuis `mentor` réussi : 0.5 point
6. 🌞 Testez l'accès au serveur web depuis la machine `etudiant` à l'aide d'une commande curl. (0.5 point)
   - Accès au serveur web depuis `etudiant` réussi : 0.5 point

#### Partie 5 : DNS (3 points)
1. 🌞 Installez un serveur DNS sur la machine `routeur`. (0.5 point)
   - Serveur DNS installé : 0.5 point
2. 🌞 Configurez le serveur DNS pour qu'il puisse résoudre les noms de domaine des machines `etudiant` et `mentor`. (1 point)
   - DNS configuré pour résoudre `etudiant` et `mentor` : 1 point
3. 🌞 Testez la résolution de noms de domaine depuis la machine `etudiant`. (0.5 point)
   - Résolution de noms de domaine depuis `etudiant` réussie : 0.5 point
4. 🌞 Testez la résolution de noms de domaine depuis la machine `mentor`. (0.5 point)
   - Résolution de noms de domaine depuis `mentor` réussie : 0.5 point

### Total : 20 points