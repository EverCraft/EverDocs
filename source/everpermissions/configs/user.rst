=======
Joueurs
=======

Le fichier de configuration des joueurs se trouve dans : ``/config/everpermissions/user/<type de monde>.conf``

.. code-block:: bash

	# L'UUID du joueur
	"86f8f95b-e5e6-45c4-bf85-4d64dbd0903f" {
		# Le dernier pseudo connu 
		name="rexbut"
		
		# Le groupe
		group="ad808c28-8636-4848-94a4-54a41292ac0d"
		
		# La liste des permissions
		# "<permission>"=<true|false>
		# True : Le joueur aura la permission
		# False : Le joueur n'aura pas la permission
		permissions {
			"minecraft.command.op"=false
			"minecraft.command.deop"=false
		}
		
		# La liste des options
		# "<key>"="<value>"
		options {
			"hover"="&7Ping : &a{PING}&7 ms[RT]&7Connecté depuis : &a{LAST_DATE_PLAYED}"
			"prefix"="&c"
			"suggest"="/msg {NAME} "
		}

		# La liste des sous-groupes
		subgroups=[
			"c712e9ec-6aa4-407e-8fdb-7f3e36dd70b6"
		]
	}
