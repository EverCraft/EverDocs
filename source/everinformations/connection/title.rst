=====
Title
=====

.. image:: ../images/EverInformations_Newbie.png
   :height: 180px
   :width: 350px
   :alt: EverInformations Connection
   :align: right

Connection Title permet de faire afficher des titres et des sous-titres lors de la connexion d'un joueur. Il existe deux types de messages : les messages pour le nouveau joueur et les messages pour les autres joueurs qui sont déjà connectés sur le serveur.

Tous les messages sont définis dans le fichier de configuration et ils peuvent contenir des `Variables Globales <../../everapi/variables.html#variables-globales>`_ et des `Variables Joueurs <../../everapi/variables.html#variables-joueurs>`_.

Configuration simple
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/connection/connection_title.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# Le nom du groupe (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				subTitle="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
		}
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# La durée pendant la quelle les titres et les sous-titres vont rester à l'écran (en seconde) 
		stay=20
		
		# Le titre
		title=""
		
		# Le nom du groupe (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				subTitle="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
			
			# Message lors de la déconnexion du joueur
			QUIT {
				# Le message
				subTitle="&7&l[&4-&7&l] {DISPLAYNAME} &7vient de quitter le serveur"
			}
			
			# Message lors de l'expulsion du joueur
			KICK {
				# Le message
				subTitle="&7&l[&4-&7&l] {DISPLAYNAME} &7vient d'être expulser du serveur pour <reason>"
			}
		}
	}

Configuration Avancée
~~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/fr.evercraft.everinformations/connection/connection_title.conf``

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
		
		# Le nom du groupe (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# La liste des messages
				messages=[
					# Message avec titre
					{
						title="&7&l[&2+&7&l] {DISPLAYNAME}"
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
						subTitle="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
					}
				]
			}
		}
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
		
		# Le nom du groupe (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				subTitle="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
			
			# Message lors de la déconnexion du joueur
			QUIT {
				# Le message
				subTitle="&7&l[&4-&7&l] {DISPLAYNAME} &7vient de quitter le serveur"
			}
			
			# Message lors de l'expulsion du joueur
			KICK {
				# Le message
				subTitle="&7&l[&4-&7&l] {DISPLAYNAME} &7vient d'être expulser du serveur pour <reason>"
			}
		}
	}