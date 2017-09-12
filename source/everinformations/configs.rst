==============
Configurations
==============

Le fichier de configuration se trouve dans : ``/config/everinformations/config.conf``

.. code-block:: bash

	# Affiche les performances du plugin dans les logs
	DEBUG=false
	
	# Permet de choisir la langue des messages
	#   French : FR_fr
	#   English : EN_en
	LANGUAGE="FR_fr"
	
	# Permet d'afficher les messages de bienvenue et de connexion en même temps pour les nouveaux joueurs
	#   True : Newbie et Connection
	#   False : Newbie uniquement
	newbie-and-connection=false
	
	# Permet de faire afficher des faux messages de déconnexion et de connexion 
	# lors qu'un joueur active ou désative son vanish
	#   True : Affichera des faux messages de déconnexion et de connexion
	#   False : Affichera aucun message
	vanish-connection-fake=true
