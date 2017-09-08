====
Chat
====

.. image:: ../images/EverInformations_Newbie.png
   :height: 180px
   :width: 350px
   :alt: EverInformations Newbie
   :align: right

Le Newbie Chat permet de faire afficher dans le tChat des messages lors de la première connexion d'un joueur. Il existe deux types de messages : les messages pour le nouveau joueur et les messages pour les autres joueurs qui sont déjà connectés sur le serveur.

Tous les messages sont définis dans le fichier de configuration et ils peuvent contenir des `Variables Globales <../../everapi/variables.html#variables-globales>`_ et des `Variables Joueurs <../../everapi/variables.html#variables-joueurs>`_.

Configuration simple
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/newbie/newbie_chat.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le message
		message="&4Bienvenue &6{DISPLAYNAME} &4sur le serveur &6{SERVER_NAME} &4!"
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le message
		message="&6{DISPLAYNAME} &4est un nouveau joueur !"
	}

Configuration Avancée
~~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/newbie/newbie_chat.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps entre chaque message (en seconde)
		interval=0
		
		# Le préfixe uniquement pour ce message ("" : Aucun préfixe)
		prefix="[&4Ever&6&lInformations&f] "
		
		# La liste des messages
		messages=[
			# Configuration normale
			"&4Bienvenue &a{DISPLAYNAME} &4sur le serveur &6{SERVER_NAME} &c!",
			
			# Configuration avancée
			{
				# Le temps avant le prochaine message (en seconde)
				next=20
				
				# Le préfixe uniquement pour ce message ("" : Aucun préfixe)
				prefix=""
				
				# Le format du message : FORMATTING_CODE|JSON (Format par défaut : FORMATTING_CODE)
				format="FORMATTING_CODE"
				
				# Le message en FORMATTING_CODE
				message="&cMessage 2 à  ......"
			},
			
			# Configuration normale
			"&bMessage 3 ......"
		]
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps entre chaque message (en seconde)
		interval=0
		
		# Le préfixe uniquement pour ce message
		prefix="[&4Ever&6&lInformations&f] "
		
		# La liste des messages
		messages=[
			# Configuration normale
			"&a{DISPLAYNAME} &4est un nouveau joueur !",
			
			# Configuration avancée
			{
				# Le temps avant le prochaine message (en seconde)
				next=20
				
				# Le préfixe uniquement pour ce message
				prefix=""
				
				# Le format du message : FORMATTING_CODE|JSON (Format par défaut : FORMATTING_CODE)
				format="JSON"
				
				# Le message en JSON
				message="{\"hoverEvent\":{\"action\":\"show_text\",\"value\":\"Message Hover\"},\"text\":\"Message en JSON\"}"
			},
			
			# Configuration normale
			"&bMessage 3 ......"
		]
	}