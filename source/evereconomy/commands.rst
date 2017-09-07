=========
Commandes
=========

.. note::
	- **<argument> :** argument obligatoire
	- **[argument] :** argument optionnel
	
La liste des commandes du plugin EverEconomy.

Générale
~~~~~~~~

Gestion du plugin
-----------------
- **Commande :** ``/evereconomy <help|reload|give|take|reset>``
- **Alias :** evereco, eco
- **Description :** 
	- **help :** Affiche l'aide du plugin
	- **reload :** Recharge le plugin
	- **give <joueur> <quantité> :** Donner de la monnaie à un joueur
	- **take <joueur> <quantité> :** Retirer de le monnaie à un joueur
	- **reset <joueur> :** Réinitialiser le solde d'un joueur
- **Permissions :** 
	- ``evereconomy.commands.execute``
	- ``evereconomy.commands.help``
	- ``evereconomy.commands.reload``
	- ``evereconomy.commands.give``
	- ``evereconomy.commands.take``
	- ``evereconomy.commands.reset``
	
Joueur
~~~~~~
	
Solde du compte
---------------
- **Commande :** ``/balance [joueur]``
- **Description :** Permet de connaître le solde d'un joueur
- **Permission :** 
	- ``evereconomy.commands.balance.execute``
	- ``evereconomy.commands.balance.others``
- **Exemple :** */balance rexbut*

Balance Top 
-----------
- **Commande :** ``/balancetop``
- **Description :** Permet de lister les joueurs possédant le plus de monnaie
- **Permission :** ``evereconomy.commands.balancetop.execute``
	
Payer un joueur
---------------
- **Commande :** ``/pay <joueur> <quantité>``
- **Description :** Permet d'envoyer de la monnaie à un autre joueur
- **Permission :** ``evereconomy.commands.pay.execute``
