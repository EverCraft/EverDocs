=======
Groupes
=======

.. note::
	- **<argument> :** argument obligatoire
	- **[argument] :** argument optionnel
	
La liste des commandes du plugin EverPermissions.

Générale
~~~~~~~~

Créer un groupe
---------------
- **Commande :** ``/permgadd <groupe> [monde]``
- **Alias :** mangadd
- **Description :** Ajoute un groupe à un monde
- **Permission :** ``everpermissions.commands.group.group.add``
- **Exemple :** */permgadd Admin*

Supprimer un groupe
-------------------
- **Commande :** ``/permgdel <joueur> [monde]``
- **Alias :** mangdel
- **Description :** Supprime un groupe d'un monde
- **Permission :** ``everpermissions.commands.group.group.del``
- **Exemple :** */permgdel Admin*

Groupe par défaut
-----------------
- **Commande :** ``/permgdefault <groupe> <true|false> [monde]``
- **Alias :** mangdefault
- **Description :** Définit un groupe par défaut
- **Permission :** ``everpermissions.commands.group.group.default``
- **Exemple :** */permgdefault Default true*

Liste des groupes
-----------------
- **Commande :** ``/permglist [monde]``
- **Alias :** permglistg, manglist
- **Description :** Affiche la liste des groupes d'un monde
- **Permission :** ``everpermissions.commands.group.group.list``
- **Exemple :** */permglist*

Gestion des inheritances
~~~~~~~~~~~~~~~~~~~~~~~~

Ajouter une inhéritance
-----------------------
- **Commande :** ``/permgaddi <groupe> <inheritance> [monde]``
- **Alias :** mangaddi
- **Description :** Ajoute une inhéritance à un groupe
- **Permission :** ``everpermissions.commands.group.inheritance.add``
- **Exemple :** */permgaddi Admin Moderator*

Retirer une inhéritance
-----------------------
- **Commande :** ``/permgdeli <groupe> <inheritance> [monde]``
- **Alias :** mangdeli
- **Description :** Supprime une inhéritance d'un groupe
- **Permission :** ``everpermissions.commands.group.inheritance.del``
- **Exemple :** */permgdeli Admin Moderator*

Liste des inhéritances
----------------------
- **Commande :** ``/permglist <groupe> [monde]``
- **Alias :** permglistg, manglist
- **Description :** Affiche la liste des inhéritances d'un groupe
- **Permission :** ``everpermissions.commands.group.inheritance.list``
- **Exemple :** */permuaddsub Admin*

Gestion des permissions
~~~~~~~~~~~~~~~~~~~~~~~

Ajouter une permission
----------------------
- **Commande :** ``/permgaddp <groupe> <permission> <true|false> [monde]``
- **Alias :** mangaddp
- **Description :** Ajoute une permission à un groupe
- **Permission :** ``everpermissions.commands.group.permission.add``
- **Exemple :** */permgaddp Admin everessentials.commands.ping.execute true*

Retirer une permission
----------------------
- **Commande :** ``/permgdelp <groupe> <permission> [monde]``
- **Alias :** mangdelp
- **Description :** Retire une permission à un groupe
- **Permission :** ``everpermissions.commands.group.permission.del``
- **Exemple :** */permgdelp Admin everessentials.commands.ping.execute*

Vérifier une permission
-----------------------
- **Commande :** ``/permgcheckp <groupe> <permission> [monde]``
- **Alias :** mangcheckp
- **Description :** Vérifie si un groupe a une permission
- **Permission :** ``everpermissions.commands.group.permission.check``
- **Exemple :** */permgcheckp Admin everessentials.commands.ping.execute*

Liste des permissions
---------------------
- **Commande :** ``/permglistp <groupe> [monde]``
- **Alias :** manglistp
- **Description :** Affiche la liste des permissions d'un groupe
- **Permission :** ``everpermissions.commands.group.permission.list``
- **Exemple :** */permglistp Admin*

Gestion des options
~~~~~~~~~~~~~~~~~~~

Ajouter une option
------------------
- **Commande :** ``/permgaddo <groupe> <option> <value> [monde]``
- **Alias :** mangaddo, mangaddv
- **Description :** Ajoute une option à un groupe
- **Permission :** ``everpermissions.commands.group.option.add``
- **Exemple :** */permuaddo rexbut prefix &c*

Retirer une option
------------------
- **Commande :** ``/permgdelo <groupe> <option> [monde]``
- **Alias :** mangdelo, mangdelv
- **Description :** Supprime une option à un groupe
- **Permission :** ``everpermissions.commands.group.option.del``
- **Exemple :** */permudelo rexbut prefix*

Vérifier une option
-------------------
- **Commande :** ``/permgchecko <groupe> <option> [monde]``
- **Alias :** mangchecko, mangcheckv
- **Description :** Vérifie si un groupe a une option
- **Permission :** ``everpermissions.commands.group.option.check``
- **Exemple :** */permuchecko rexbut prefix*

Liste des options
-----------------
- **Commande :** ``/permglisto <groupe> [monde]``
- **Alias :** manglisto, manglistv
- **Description :** Affiche la liste des options d'un groupe
- **Permission :** ``everpermissions.commands.group.option.list``
- **Exemple :** */permulisto rexbut*
