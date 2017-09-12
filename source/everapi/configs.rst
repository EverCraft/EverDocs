==============
Configurations
==============

Le fichier de configuration se trouve dans : ``/config/everapi/config.conf``

.. code-block:: bash

	# Affiche les performances du plugin dans les logs
	DEBUG=false
	
	# Permet de choisir la langue des messages
	#   French : FR_fr
	#   English : EN_en
	LANGUAGE="FR_fr"
	
	# Permet de désactiver des commandes du plugin
	DISABLE-COMMANDS=[
		"command_name"
	]
	
	# Le nom du serveur (Utilisé dans les variables globales)
	server-name=EverCraft
	
	# Le nombre maximum de caractere pour un nom de HOME, de JAIL...
	max-caractere=16
	
	# Le format de la date (https://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html)
	format {
		date="dd MMM yyyy"
		datetime="dd MMM yyyy HH:mm:ss"
		time="HH:mm"
	}
	
	# Utilisé pour vérifier si les arguments d'une commande sont correctes
	location {
		maxX=30000
		maxY=255
		maxZ=30000
		minX=-30000
		minY=0
		minZ=-30000
	}
	
	# Définissez à TRUE pour activer l'utilisation des permissions pour accès à monde
	# Permission : everapi.worlds.<worldname>
	# Utilisé par les commands (world, home, tp...)
	world-permissions=false
