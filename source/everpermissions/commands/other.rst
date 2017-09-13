=============
Autre subject
=============

.. note::
	- **<argument> :** argument obligatoire
	- **[argument] :** argument optionnel
	
La liste des commandes du plugin EverPermissions.

Gestion des groupes
~~~~~~~~~~~~~~~~~~~

Définir un groupe
-----------------
- **Commande :** ``/permoaddg <collection> <subject> <groupe> [monde]``
- **Alias :** permoadd, manoadd, manoaddg
- **Description :** Défini le groupe d'un subject
- **Permission :** ``everpermissions.commands.other.group.add``
- **Exemple :** */permoaddg rexbut Admin*

Retirer le groupe
-----------------
- **Commande :** ``/permodelg <collection> <subject> [monde]``
- **Alias :** permodelg, manodel, manodel
- **Description :** Supprime le groupe d'un subject
- **Permission :** ``everpermissions.commands.other.group.del``
- **Exemple :** */permodelg rexbut*

Ajouter un sous-groupe
----------------------
- **Commande :** ``/permoaddsub <collection> <subject> <sous-groupe> [monde]``
- **Alias :** manoaddsub
- **Description :** Ajoute un sous-groupe à un subject
- **Permission :** ``everpermissions.commands.other.group.addsub``
- **Exemple :** */permoaddsub rexbut Moderator*

Retirer un sous-groupe
----------------------
- **Commande :** ``/permodelsub <collection> <subject> <sous-groupe> [monde]``
- **Alias :** manodelsub
- **Description :** Supprime un sous-groupe à un subject
- **Permission :** ``everpermissions.commands.other.group.delsub``
- **Exemple :** */permodelsub rexbut Moderator*

Promouvoir
----------
- **Commande :** ``/permopromote <collection> <subject> <groupe> [monde]``
- **Alias :** manopromote
- **Description :** Promouvoit un subject
- **Permission :** ``everpermissions.commands.other.group.promote``
- **Exemple :** */permopromote rexbut Admin*

Rétrograder
-----------
- **Commande :** ``/permodemote <collection> <subject> <groupe> [monde]``
- **Alias :** manodemote
- **Description :** Rétrograde un subject
- **Permission :** ``everpermissions.commands.other.group.demote``
- **Exemple :** /permodemote rexbut Moderator

Liste des groupes
-----------------
- **Commande :** ``/permolistg <collection> <subject> [monde]``
- **Alias :** permolistg
- **Description :** Affiche la liste des groupes d'un subject
- **Permission :** ``everpermissions.commands.other.group.list``
- **Exemple :** */permolistg rexbut*

Gestion des permissions
~~~~~~~~~~~~~~~~~~~~~~~

Ajouter une permission
----------------------
- **Commande :** ``/permoaddp <collection> <subject> <permission> <true|false> [monde]``
- **Alias :** manoaddp
- **Description :** Ajoute une permission à un subject
- **Permission :** ``everpermissions.commands.other.permission.add``
- **Exemple :** */permoaddp rexbut everessentials.commands.ping.execute true*

Retirer une permission
----------------------
- **Commande :** ``/permodelp <collection> <subject> <permission> [monde]``
- **Alias :** manodelp
- **Description :** Retire une permission à un subject
- **Permission :** ``everpermissions.commands.other.permission.del``
- **Exemple :** */permodelp rexbut everessentials.commands.ping.execute*

Vérifier une permission
-----------------------
- **Commande :** ``/permocheckp <collection> <subject> <permission> [monde]``
- **Alias :** manocheckp
- **Description :** Vérifie si un subject a une permission
- **Permission :** ``everpermissions.commands.other.permission.check``
- **Exemple :** */permocheckp rexbut everessentials.commands.ping.execute*

Liste des permissions
----------------------
- **Commande :** ``/permolistp <collection> <subject> [monde]``
- **Alias :** manolistp
- **Description :** Affiche la liste des permissions d'un subject
- **Permission :** ``everpermissions.commands.other.permission.list``
- **Exemple :** */permolistp rexbut*

Gestion des options
~~~~~~~~~~~~~~~~~~~

Ajouter une option
------------------
- **Commande :** ``/permoaddo <collection> <subject> <option> <value> [monde]``
- **Alias :** manoaddp
- **Description :** Ajoute ou remplace une option à un subject
- **Permission :** ``everpermissions.commands.other.option.add``
- **Exemple :** */permoaddo rexbut prefix &c*

Retirer une option
------------------
- **Commande :** ``/permodelo <collection> <subject> <option> [monde]``
- **Alias :** manodelp
- **Description :** Supprime une option à un subject
- **Permission :** ``everpermissions.commands.other.option.del``
- **Exemple :** */permodelo rexbut prefix*

Vérifier une option
-------------------
- **Commande :** ``/permochecko <collection> <subject> <option> [monde]``
- **Alias :** manocheckp
- **Description :** Vérifie si un subject a une option
- **Permission :** ``everpermissions.commands.other.option.check``
- **Exemple :** */permochecko rexbut prefix*

Liste des options
-----------------
- **Commande :** ``/permolisto <collection> <subject> [monde]``
- **Alias :** manolistp
- **Description :** Affiche la liste des options d'un subject
- **Permission :** ``everpermissions.commands.other.option.list``
- **Exemple :** */permolisto rexbut*
