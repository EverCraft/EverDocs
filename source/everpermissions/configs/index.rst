==============
Configurations
==============

Par défaut les informations sont sauvegardées dans des fichiers de configuration. Cependant si vous avez activé le mode base de données, uniquement les groupes seront encore sauvegardés en fichier. Les autres informations seront enregistrées directement dans la base de données.

.. toctree::
   :maxdepth: 1
   
   group
   user
   system
   commandblock

Le fichier de configuration principal se trouve dans : ``/config/everpermissions/config.conf``

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
	
	# Permet de choisir où seront sauvegardés les données (Sauf les groupes qui seront toujours en fichier)
	# Par défaut des données sont sauvegarder en fichier .conf	
	SQL {
		# Permets d'activer ou de désactiver la fonctionnalité 
		enable=false
		
		# Le nom qui sera mis devant toutes les Tables
		prefix="EverEconomy_"
		
		# L'URL de la base de données
		#   H2 : "jdbc:h2:~/config/evereconomy/data"
		#   SQL : "jdbc:mysql://[login[:password]@]{host}:{port}/{database}"
		url="jdbc:mysql://root:password@localhost:3306/minecraft"
	}
	
	# EverPermissions permet d'avoir des permissions différentes par monde.
	# Vous pouvez regrouper des mondes qu'ils aient les mêmes permissions
	# Exemple : (Le monde 'world' et 'DIM1' auront les mêmes permissions mais pas 'DIM-1')
	#   default=[
	#     "world",
	#     "DIM1"
	#   ],
	#   type-nether=[
	#     "DIM-1"
	#   ]
	collections {
		# La liste des mondes pour groupes
		group {
			default=[
				"world",
				"DIM1",
				"DIM-1"
			]
		}
		
		# La liste des mondes pour joueurs
		user {
			default=[
				"world",
				"DIM1",
				"DIM-1"
			]
		}
		
		# La liste des mondes pour le System (Console, RCON)
		# Il est conseillé de laisser les valeurs par défaut pour le System 
		# car le monde n'est jamais connu
		system {
			default=[
				"world",
				"DIM1",
				"DIM-1"
			]
		}

		# La liste des mondes pour les CommandeBlocs
		commandblock {
			default=[
				"world",
				"DIM1",
				"DIM-1"
			]
		}
	}