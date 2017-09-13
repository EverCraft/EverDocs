=========
Priorités
=========

Le service de priority permet de gérér les priorités des fonctionnalités.

Le fichier de configuration se trouve dans : ``/config/everapi/priority.conf``

Spawn
~~~~~

Cela permet de gérer la priorité du respawn des joueurs.

.. code-block:: bash

	spawn=[
		# Le spawn des nouveaux joueur (Fournit par EverEssentials)
		"newbie",
		
		# Le spawn de la région (Fournit par EverWorldGuard)
		"everworldguard",
		
		# Le Home du joueur (Fournit par EverEssentials)
		"home",
		
		# Le spawn du group du joueur (Fournit par EverEssentials)
		"spawn",
		
		# Le lit du joueur (Fournit par MineCraft)
		"bed",
		
		# Le spawn du monde (Fournit par MineCraft)
		"world"
	]
	
Message
~~~~~~~

Cela permet gérer la priorité d'affichage des messages.

.. code-block:: bash

	"actionbar, bossbar, title"=[
		# Le message de sanction de Mute (Fournit par EverSanctions)
		"eversanctions.mute",
		
		# Le message de sanction de Jail (Fournit par EverSanctions)
		"eversanctions.jail",
		
		# Le message de bienvenu pour le nouveau joueur (Fournit par EverInformations)
		"everinformations.newbie.player",
		
		# Le message de bienvenu pour les autres joueurs (Fournit par EverInformations)
		"everinformations.newbie.others",
		
		# Le message de connexion pour le joueur(Fournit par EverInformations)
		"everinformations.connection.player",
		
		# Le message de connexion pour les autres joueurs (Fournit par EverInformations)
		"everinformations.connection.others",
		
		# Les autres messages
		"message",
		
		# Les messages de worldguard (Fournit par EverWorldGuard)
		"everworldguard",
		
		# Les messages d'annonce (Fournit par EverInformations)
		"everinformations.automessages"
	]

Autres
~~~~~~

Cela permet de gérer la priorité d'autres fonctionnalités.

.. code-block:: bash

	# La priorité du NameTag
	"nametag"=[
		# Le NameTag d'EverInformations
		"everinformations"
	]
	
	# La priorité du TabList
	"tablist"=[
		# Le TabList d'EverInformations
		"everinformations"
	]
	
	# La priorité du ScoreBoard BelowName
	"scoreboard:below_name"=[
		# Le ScoreBoard BelowName d'EverInformations
		"everinfo.below"
	]
	
	
	# La priorité du ScoreBoard List
	"scoreboard:list"=[
		# Le ScoreBoard List d'EverInformations
		"everinfo.list"
	]
	
	
	# La priorité du ScoreBoard Sidebar
	"scoreboard:sidebar"=[
		# Le ScoreBoard Sidebar d'EverInformations
		"everinfo.sidebar"
	]