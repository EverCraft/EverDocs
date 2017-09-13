=======
Systems
=======

Le fichier de configuration du System se trouve dans : ``/config/everpermissions/system/<type de monde>.conf``

.. code-block:: bash

	# Le nom du system
	"system" {
		# L'Alias
		name="System"
		
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
			"prefix"="&c"
		}

		# La liste des sous-groupes
		subgroups=[
			"c712e9ec-6aa4-407e-8fdb-7f3e36dd70b6"
		]
	}
