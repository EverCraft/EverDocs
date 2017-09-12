==============
Configurations
==============

Le fichier de configuration se trouve dans : ``/config/everchat/config.conf``

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
	
	# Permets d'activer ou de désactiver la fonctionnalité des Icônes
	icons-enable=true
	
	# La mise en forme du tChat
	format {
		# Permets d'activer ou de désactiver la fonctionnalité de la mise en forme du tChat
		enable=true
		
		# Le format des messages pour les joueurs par défaut
		default="{DISPLAYNAME} &7:&f {MESSAGE}"
		
		# Le format des messages selon les groupes
		groups {
			# Format pour un groupe
			Admin="&f[&4Admin&f] {DISPLAYNAME} &7:&f {MESSAGE}"
			
			# Format pour un groupe
			Moderator="&f[&5Moderator&f] {DISPLAYNAME} &7:&f {MESSAGE}"
		}
	}

	# La liste des élements qui seront remplacé dans les messages
	replaces {
		"[*]"="✖"
		"[<3]"="❤"
		"[ARROW]"="➜"
		"[RT]"="\n"
		"[X]"="█"
		"[check]"="✔"
	}
