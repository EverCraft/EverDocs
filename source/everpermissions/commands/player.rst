=======
Joueurs
=======

.. note::
	- **<argument> :** argument obligatoire
	- **[argument] :** argument optionnel
	
La liste des commandes du plugin EverPermissions.

Générale
~~~~~~~~

Réinitialiser un joueur
-----------------------
- **Commande :** ``/permuclear <joueur>``
- **Alias :** manuclear
- **Description :** Réinitialise tous les données d'un joueur
- **Permission :** ``everpermissions.commands.user.clear``
- **Exemple :** */permuclear rexbut*

Gestion des groupes
~~~~~~~~~~~~~~~~~~~

Définir un groupe
-----------------
- **Commande :** ``/permuaddg <joueur> <groupe> [monde]``
- **Alias :** permuadd, manuadd, manuaddg
- **Description :** Défini le groupe d'un joueur
- **Permission :** ``everpermissions.commands.user.group.add``
- **Exemple :** */permuaddg rexbut Admin*

Retirer le groupe
-----------------
- **Commande :** ``/permudelg <joueur> [monde]``
- **Alias :** permudelg, manudel, manudel
- **Description :** Supprime le groupe d'un joueur
- **Permission :** ``everpermissions.commands.user.group.del``
- **Exemple :** */permudelg rexbut*

Ajouter un sous-groupe
----------------------
- **Commande :** ``/permuaddsub <joueur> <sous-groupe> [monde]``
- **Alias :** manuaddsub
- **Description :** Ajoute un sous-groupe à un joueur
- **Permission :** ``everpermissions.commands.user.group.addsub``
- **Exemple :** */permuaddsub rexbut Moderator*

Retirer un sous-groupe
----------------------
- **Commande :** ``/permudelsub <joueur> <sous-groupe> [monde]``
- **Alias :** manudelsub
- **Description :** Supprime un sous-groupe à un joueur
- **Permission :** ``everpermissions.commands.user.group.delsub``
- **Exemple :** */permudelsub rexbut Moderator*

Promouvoir
----------
- **Commande :** ``/permupromote <joueur> <groupe> [monde]``
- **Alias :** permpromote, manpromote, manupromote
- **Description :** Promouvoit un joueur
- **Permission :** ``everpermissions.commands.user.group.promote``
- **Exemple :** */permupromote rexbut Admin*

Rétrograder
-----------
- **Commande :** ``/permudemote <joueur> <groupe> [monde]``
- **Alias :** permdemote, mandemote, manudemote
- **Description :** Rétrograde un joueur
- **Permission :** ``everpermissions.commands.user.group.demote``
- **Exemple :** /permudemote rexbut Moderator

Lister des groupes
------------------
- **Commande :** ``/permulistg <joueur> [monde]``
- **Alias :** permulistg, manwhois
- **Description :** Affiche la liste des groupes d'un joueur
- **Permission :** ``everpermissions.commands.user.group.list``
- **Exemple :** */permulistg rexbut*

Gestion des permissions
~~~~~~~~~~~~~~~~~~~~~~~

Ajouter une permission
----------------------
- **Commande :** ``/permuaddp <joueur> <permission> <true|false> [monde]``
- **Alias :** manuaddp
- **Description :** Ajoute une permission à un joueur
- **Permission :** ``everpermissions.commands.user.permission.add``
- **Exemple :** */permuaddp rexbut everessentials.commands.ping.execute true*

Retirer une permission
----------------------
- **Commande :** ``/permudelp <joueur> <permission> [monde]``
- **Alias :** manudelp
- **Description :** Retire une permission à un joueur
- **Permission :** ``everpermissions.commands.user.permission.del``
- **Exemple :** */permudelp rexbut everessentials.commands.ping.execute*

Vérifier une permission
-----------------------
- **Commande :** ``/permucheckp <joueur> <permission> [monde]``
- **Alias :** manucheckp
- **Description :** Vérifie si un joueur a une permission
- **Permission :** ``everpermissions.commands.user.permission.check``
- **Exemple :** */permucheckp rexbut everessentials.commands.ping.execute*

Lister des permissions
----------------------
- **Commande :** ``/permulistp <joueur> [monde]``
- **Alias :** manulistp
- **Description :** Affiche la liste des permissions d'un joueur
- **Permission :** ``everpermissions.commands.user.permission.list``
- **Exemple :** */permulistp rexbut*

Gestion des options
~~~~~~~~~~~~~~~~~~~

Ajouter une option
------------------
- **Commande :** ``/permuaddo <joueur> <option> <value> [monde]``
- **Alias :** manuaddp
- **Description :** Ajoute ou remplace une option à un joueur
- **Permission :** ``everpermissions.commands.user.option.add``
- **Exemple :** */permuaddo rexbut prefix &c*

Retirer une option
------------------
- **Commande :** ``/permudelo <joueur> <option> [monde]``
- **Alias :** manudelp
- **Description :** Supprime une option à un joueur
- **Permission :** ``everpermissions.commands.user.option.del``
- **Exemple :** */permudelo rexbut prefix*

Vérifier une option
-------------------
- **Commande :** ``/permuchecko <joueur> <option> [monde]``
- **Alias :** manucheckp
- **Description :** Vérifie si un joueur a une option
- **Permission :** ``everpermissions.commands.user.option.check``
- **Exemple :** */permuchecko rexbut prefix*

Lister des options
------------------
- **Commande :** ``/permulisto <joueur> [monde]``
- **Alias :** manulistp
- **Description :** Affiche la liste des options d'un joueur
- **Permission :** ``everpermissions.commands.user.option.list``
- **Exemple :** */permulisto rexbut*
