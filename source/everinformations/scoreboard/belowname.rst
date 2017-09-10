=========
BelowName
=========

.. image:: ../images/EverInformations_ScoreBoard_BelowName.gif
   :height: 180px
   :width: 350px
   :alt: EverInformations ScoreBoard List
   :align: right

Le ScoreBoard BelowName permet de faire affiché une information au dessus de chaque joueur. L'information est composé d'un nombre et d'un message. 

Le nombre à afficher doit être pris dans `la liste des Scores <../../everapi/scores.html>`_ (Exemple : HEALTH, PING, BALANCE...), il sera automatique actualiser.

Configuration simple
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/everinformations/scoreboard/scoreboard_belowname.conf``

.. code-block:: bash
	
	# Permets d'activer ou de désactiver la fonctionnalité
	enable=true
	
	# Le Score qui sera affiché : (HEALTH|BALANCE|PING|FOOD...)
	type=HEALTH
	
	# Le message qui sera affiché à droite du nombre
	name="&4❤"
	
Configuration Avancée
~~~~~~~~~~~~~~~~~~~~

Le fichier de configuration se trouve dans : ``/config/everinformations/scoreboard/scoreboard_belowname.conf``

.. code-block:: bash
	
	# Permets d'activer ou de désactiver la fonctionnalité
	enable=true
	
	# Le temps d'apparition de chaque objective en seconde (Par défaut : 60)
	stay=60
	
	# Le délais d'actualisation des Scores qui ne sont pas automatique (PING) en seconde (Par défaut : 20)
	update=30
	
	# La liste des objectives qui seront affiché chaqu'un leur tour
	objectives=[
		# Configuration simple
		{
			# Le Score qui sera affiché dans cet objective :
			type=HEALTH
			
			# Le message pour cet objective
			name="&4❤"
		},
		
		# Configuration avancée
		{
			# Le Score qui sera affiché dans cet objective :
			type=PING
			
			# Le message pour cet objective
			name="&4ms"
			
			# Le temps d'apparition de cet objective en seconde
			stay=30
			
			# Le délais d'actualisation cet objective
			update=5
		}
	]