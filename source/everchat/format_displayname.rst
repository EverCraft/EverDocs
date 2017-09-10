=======================
Mise en forme du pseudo
=======================

.. image:: images/EverChat_format.png
   :height: 180px
   :width: 350px
   :alt: EverChat description
   :align: right

Le "DISPLAYNAME" est le nom du joueur avec le préfixe, le suffixe, le hover et le suggest. 

Tous les éléments sont fourni par le service de Permission, donc cela signifie qu'il peut-être défini soit : 
	- par dans un groupe
	- pour un joueur spécifique 

Prefix
~~~~~~

Le préfixe est ajouté avant le pseudo du joueur : "**[Prefix]pseudo**".

La valeur du préfixe est récupéré à partir de l'option "**prefix**" fournit par le service de permission.

**Exemple pour le plugin EverPermissions :**

- Pour ajouter à un groupe : ``/permgaddo <groupe> prefix <valeur>``
- Pour ajouter à un joueur : ``/permuaddo <joueur> prefix <valeur>``

Suffix
~~~~~~

Le suffixe est ajouté après le pseudo du joueur : "pseudo[Suffix]"

La valeur du préfixe est récupéré à partir de l'option "suffix" fournit par le service de permission.

**Exemple pour le plugin EverPermissions :**

- Pour ajouter à un groupe : ``/permgaddo <groupe> suffix <valeur>``
- Pour ajouter à un joueur : ``/permuaddo <joueur> suffix <valeur>``

Hover
~~~~~

Il est possible d'afficher un message lorsque l'on survole le "DisplayName".

La valeur du hover est récupéré à partir de l'option "hover" fournit par le service de permission.

**Exemple pour le plugin EverPermissions :**

- Pour ajouter à un groupe : ``/permgaddo <groupe> hover <valeur>``
- Pour ajouter à un joueur : ``/permuaddo <joueur> hover <valeur>``

Suggest
~~~~~~~

Il est possible de suggérer une commande lorsque l'on clique sur le "DisplayName".

La valeur du suggest est récupéré à partir de l'option "suggest" fournit par le service de permission.

**Exemple pour le plugin EverPermissions :**

- Pour ajouter à un groupe : ``/permgaddo <groupe> suggest <valeur>``
- Pour ajouter à un joueur : ``/permuaddo <joueur> suggest <valeur>``
