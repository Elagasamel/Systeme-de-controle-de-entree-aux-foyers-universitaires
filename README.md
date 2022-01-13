# Syst-me-de-contr-le-d-entr-e-aux-foyers-universitaires---base-de-RFID
 Ce projet propose un prototype de conception du système, la mise en œuvre et la  description des outils et des technologies nécessaires pour développer une RFID (Radio Frequency Identification) dédiée pour contrôler l’accès des étudiants au  foyers universitaires, un système pour faciliter la vérification gratuite et rapide des  données liés aux étudiants ainsi que le personnel administratif.

Vous devrez installer Node.js, NodeRED et Mosquitto mqtt broker pour que ce projet fonctionne. Faites-les installer en fonction de la configuration système requise. Ce projet est compatible avec les cartes Mifare 1k et 4k. Nous devons garder Mosquitto et NodeRED en cours d'exécution dans vos terminaux.
Ensuite, ouvrir NodeRED dans votre navigateur à 127.0.0.1:1880 et importer le flux NodeRED.
Si vous exécuter Linux et que Mosquitto ne parvient pas à démarrer, exécutez sudo pkill mosquitto.
1.	Connexion aux cartes :
Connecter la carte NodeMCU au module MFRC522 de la manière suivante :
NodeMCU MFRC522
D1 ----> RST
3V3 ----> 3.3V
D8 ----> SDA
D5 ----> SCK
D6 ----> MISO
D7 ----> MOSI
GND ----> GND \

2.	Écriture des données des élèves sur des cartes 

Télécharger le sektch write_student_info sur la carte NodeMCU et ouvrez le moniteur série. Entrer ensuite les informations se terminant par « #» et appuyer sur Entrée. \




3.	Lecture des données des élèves à partir de cartes 
Télécharger notre travail dans notre  dossier  et configurer le reste du projet comme mentionné ci-dessus.


4.	Gestion des erreurs 
Appuyer sur le bouton de réinitialisation du NodeMCU en cas de problème.
