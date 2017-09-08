=====
Title
=====

.. image:: ../images/EverInformations_Newbie.png
   :height: 180px
   :width: 350px
   :alt: EverInformations Newbie
   :align: right

Newbie Title permet de faire afficher des titres et des sous-titres lors de la première connexion d'un joueur. Il existe deux types de messages : les messages pour le nouveau joueur et les messages pour les autres joueurs qui sont déjà connectés sur le serveur.

Tous les messages sont définis dans le fichier de configuration et ils peuvent contenir des `Variables Globales <../../everapi/variables.html#variables-globales>`_ et des `Variables Joueurs <../../everapi/variables.html#variables-joueurs>`_.

Configuration simple
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/newbie/newbie_title.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# Le titre
		title="&6✖ &4Bienvenue &6✖"
		
		# Le sous-titre
		subTitle="&4Bienvenue &a{DISPLAYNAME} &4sur le serveur {SERVER_NAME} !"
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# Le titre
		title=""
		
		# Le sous-titre
		subTitle="&a{DISPLAYNAME} &4est un nouveau joueur !"
	}

Configuration Avancée
~~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/newbie/newbie_title.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps entre chaque message (en seconde)
		interval=0
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# La durée du fondu d'apparition (en seconde)
		fadeIn=1
		
		# La durée du fondu de sortie (en seconde)
		fadeOut=1
		
		# La liste des messages
		messages=[
			# Message avec titre
			{
				title="&4Bienvenue &a{DISPLAYNAME} &4sur le serveur {SERVER_NAME} !"
			},
			
			# Configuration avancée
			{
				# Le temps avant le prochaine message (en seconde)
				next=20
				
				# Le format du message : FORMATTING_CODE|JSON (Format par défaut : FORMATTING_CODE)
				format="FORMATTING_CODE"
				
				# Le message en FORMATTING_CODE
				subTitle="&cMessage 2 à  ......"
			},
			
			# Message avec sous-titre
			{
				subTitle="&bMessage 3 ......"
			}
		]
	}
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps entre chaque message (en seconde)
		interval=0
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# La durée du fondu d'apparition (en seconde)
		fadeIn=1
		
		# La durée du fondu de sortie (en seconde)
		fadeOut=1
		
		# La liste des messages
		messages=[
			# Message avec titre
			{
				title="&4Bienvenue &a{DISPLAYNAME} &4sur le serveur {SERVER_NAME} !"
			},
			
			# Configuration avancée
			{
				# Le temps avant le prochaine message (en seconde)
				next=20
				
				# Le format du message : FORMATTING_CODE|JSON (Format par défaut : FORMATTING_CODE)
				format="JSON"
				
				# Le message en JSON
				subTitle="{\"hoverEvent\":{\"action\":\"show_text\",\"value\":\"Message Hover\"},\"text\":\"Message en JSON\"}"
			},
			
			# Message avec sous-titre
			{
				subTitle="&bMessage 3 ......"
			}
		]
	}