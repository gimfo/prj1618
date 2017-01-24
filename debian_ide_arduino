# Installation de l’IDE
## Vérification Java
Pour vérifier sa présence, dans un terminal, lancer la commande   :
```
java -version
```
Si java n’est pas présent, installer le package openJDK correspondant aux besoins.
OpenJDK est le portage open source de la technologie java.
sudo apt-get install openjdk-7-jdk # Kit de développement
sudo apt-get install openjdk-7-jre # Environnement d’exécution, si aucun développement en java est prévu

L’environnement d’exécution se lance automatiquement au démarrage de Linux.
Si java Sun est installé sur la distribution, il faut mettre openjdk comme version java par défaut en lançant la commande suivante autant de fois que nécessaire :
sudo update-alternatives --config java

2. Télécharger l’IDE Arduino en consultant la liste des versions disponibles
sudo wget -P /home/xavier/download http://downloads.arduino.cc/arduino-1.5.6-r2-linux64.tgz

Créer un répertoire arduino et décompresser dans celui-ci l’archive précédemment téléchargée.
sudo mkdir ~/arduino
sudo tar -C ~/arduino -xvzf ~/download/arduino-1.5.6-r2-linux64.tgz

Les dépendances gcc-avr et avr-libc sont déjà incluses dans le paquet, il n’est plus nécessaire de les installer depuis la version 1.0.1 de l’IDE Arduino.

3. Activer le port USB pour l’utilisateur.
Il est nécessaire d’enregistrer l’utilisateur courant dans le groupe dialout gérant les matériels système.
sudo usermod -aG dialout xavier

Vérifier l’affiliation au groupe
su xavier # redémarre la session utilisateur
groups # vérifie si dialout fait parti des abonnements

Brancher la carte Arduino et rechercher la connexion USB active
ls -l /dev/ttyUSB*

Modifier les droits de la connexion USB
sudo chmod a+rw /dev/ttyUSB0 # remplacer ttyUSB0 par le port USB actif lors du branchement de la carte Arduino.

Important: Remplacer ttyUSB par ttyACM pour les cartes Leonardo, UNO et très certainement toutes celles qui utilisent un port série virtuel sans circuit FTDI. ttyUSB0 est utilisé pour un Arduino Duemilanove.

4. Lancer l’IDE Arduino.
~/arduino/arduino-1.5.6-r2/arduino # Ou depuis le répertoire courant ./arduino
