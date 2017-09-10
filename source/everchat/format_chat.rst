=====================
Mise en forme du chat
=====================

.. image:: images/EverChat_format.png
   :height: 180px
   :width: 350px
   :alt: EverChat description
   :align: right

EverChat est un plugin de mise en forme du tchat. Les mises en forme utilise toutes les variables globales.

Le fichier de configuration
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Activation
----------

Prérequis :
	- Activer le formatage du tchat (``config\everchat\config.conf``)

.. code-block:: bash

	enable-format=true

Format des groupes
------------------

Il est possible de choisir un format différent pour chaque groupe :

.. code-block:: bash

	format-groups {
	   Admin="&f[&4Admin&f] <DISPLAYNAME> &7:&f <MESSAGE>"
	   Moderator="&f[&5Mod&f] <DISPLAYNAME> &7:&f <MESSAGE>"
	   Player="&f[&aPlayer&f] <DISPLAYNAME> &7:&f <MESSAGE>"
	}

Format par défaut
-----------------

Cependant si le groupe du joueur n'est pas dans la liste des groupes, le format par défaut sera appliqué :

.. code-block:: bash

	format-default="<DISPLAYNAME> &7:&f <MESSAGE>"
