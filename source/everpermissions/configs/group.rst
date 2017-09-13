======
Groupe
======

Le fichier de configuration des groupes se trouve dans : ``/config/everpermissions/group/<type de monde>.conf``

.. code-block:: bash

	# L'UUID du groupe
	"86f8f95b-e5e6-45c4-bf85-4d64dbd0903f" {
		# Le nom du groupe 
		name="Admin"
		
		# La liste des permissions
		# "<permission>"=<true|false>
		# True : Le groupe aura la permission
		# False : Le groupe n'aura pas la permission
		permissions {
			"everapi"=true
			"everchat"=true
			"evereconomy"=true
			"everessentials"=true
			"everinformations"=true
			"everpermissions"=true
			"eversigns"=true
			"everworldguard"=true
			"minecraft"=true
			"sponge"=true
		}
		
		# La liste des options
		# "<key>"="<value>"
		options {
			"hover"="&7Ping : &a{PING}&7 ms[RT]&7Connecté depuis : &a{LAST_DATE_PLAYED}"
			"prefix"="&c"
			"suggest"="/msg {NAME} "
		}

		# La liste des inhéritances
		inheritances=[
			# L'UUID du groupe Modérateur
			"c712e9ec-6aa4-407e-8fdb-7f3e36dd70b6"
		]
	}
