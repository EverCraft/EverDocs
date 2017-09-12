==============
Configurations
==============

Le fichier de configuration se trouve dans : ``/config/evereconomy/config.conf``

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
	
	# Permet de choisir où seront sauvegardés les données
	# Par défaut des données sont sauvegarder dans le fichier 'data.mv.db'
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
	
	# La configuration de la monnaie
	currency {
		# Le d'identifiant de la monnaie
		id="evereconomy_emeraude"
		
		# Le nom de la monnaie
		name="Emeraude"
		
		# Le nom de la monnaie au singulier
		singular="&aEmeraude"
		
		# Le nom de la monnaie au pluriel
		plural="&aEmeraudes"
		
		# Le symbole de la monnaie
		symbol="&aE"
		
		# Le format d'écriture de la monnaie ({amount}, {currency}, {symbol})
		format="&6{amount} {currency}"
		
		# Le solde départ d'un compte
		starting-balance=300
		
		# Le solde minimum d'un compte
		min-balance=0
		
		# Le solde maximum d'un compte
		max-balance=0
		
		# Le nombre de chiffre après la virgule
		num-fraction-digits=2
	}
	
	# La liste des joueurs qui ne seront pas dans le BalanceTop
	bypass=[
		"86f8f95b-e5e6-45c4-bf85-4d64dbd0903f"
	]