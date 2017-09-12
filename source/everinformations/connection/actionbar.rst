=========
ActionBar
=========

.. image:: ../images/EverInformations_Connection.png
   :height: 180px
   :width: 350px
   :alt: EverInformations Connection
   :align: right

Connection ActionBar permet de faire afficher des messages dans l'ActionBar lors de la connexion d'un joueur. Il existe deux types de messages : les messages pour le nouveau joueur et les messages pour les autres joueurs qui sont déjà connectés sur le serveur.

Tous les messages sont définis dans le fichier de configuration et ils peuvent contenir des `Variables Globales <../../everapi/variables.html#variables-globales>`_ et des `Variables Joueurs <../../everapi/variables.html#variables-joueurs>`_.

Configuration simple
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/everinformations/connection/connection_chat.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps d'apparition de chaque message (en seconde) 
		stay=20
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT) (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				message="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
		}
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps d'apparition de chaque message (en seconde) 
		stay=20
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				message="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
			
			# Message lors de la déconnexion du joueur
			QUIT {
				# Le message
				message="&7&l[&4-&7&l] {DISPLAYNAME} &7vient de quitter le serveur"
			}
			
			# Message lors de l'expulsion du joueur
			KICK {
				# Le message
				message="&7&l[&4-&7&l] {DISPLAYNAME} &7vient d'être expulser du serveur pour <reason>"
			}
		}
	}

Configuration Avancée
~~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/everinformations/connection/connection_chat.conf``

.. code-block:: bash

	# Pour le nouveau joueur
	player {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps entre chaque message (en seconde)
		interval=10
		
		# Le temps d'apparition de chaque message (en seconde) 
		stay=30
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				message="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
		}
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT) (ou l'UUID du groupe)
		"ad808c28-8636-4848-94a4-54a41292ac0d" {
			# Message lors de la connexion du joueur
			JOIN {				
				# Le message pour les joueurs du groupe ADMIN
				messages=[
					{
						# Le temps avant le prochaine message (en seconde)
						next=5
						
						# Le temps d'apparition de ce message (en seconde) 
						stay=15
						
						# Le format du message : FORMATTING_CODE|JSON (Format par défaut : FORMATTING_CODE)
						format="FORMATTING_CODE"
						
						# Le message
						message="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
					},
					"&4Bienvenue sur votre serveur"
				]
			}
		}
	}
	
	# Pour les autres joueurs
	others {
		# Permets d'activer ou de désactiver la fonctionnalité
		enable=true
		
		# Le temps d'apparition de chaque message (en seconde) 
		stay=30
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT)
		DEFAULT {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				message="&7&l[&2+&7&l] {DISPLAYNAME} &7vient de rejoindre le serveur"
			}
			
			# Message lors de la déconnexion du joueur
			QUIT {
				# Le message
				message="&7&l[&4-&7&l] {DISPLAYNAME} &7vient de quitter le serveur"
			}
			
			# Message lors de l'expulsion du joueur
			KICK {
				# Le message
				message="&7&l[&4-&7&l] {DISPLAYNAME} &7vient d'être expulser du serveur pour <reason>"
			}
		}
		
		# Le nom du groupe (Par défaut : DEFAULT) (Par défaut : DEFAULT) (ou l'UUID du groupe)
		"ad808c28-8636-4848-94a4-54a41292ac0d" {
			# Message lors de la connexion du joueur
			JOIN {
				# Le message
				message="&7&l[&2+&7&l] &cL'admin {DISPLAYNAME} &cvient de rejoindre le serveur"
			}
			
			# Message lors de la déconnexion du joueur
			QUIT {
				# Le message
				message="&7&l[&4-&7&l] &cL'admin {DISPLAYNAME} &cvient de quitter le serveur"
			}
		}
	}