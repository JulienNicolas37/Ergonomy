Objectifs :
============

Définir les __standards__ pour la création de beaux zécrans dans OFBiz (Uniformité)
Trouver des solutions fonctionnelles aux problèmes d'ergonomie


Comment on procède : 
--------------------

On se base sur un composant standart (partymgr) et on défini sur cet exemple les solutions design à implémenter (graphiquement).

Ensuite on implémente un nouveau plugin mettant en oeuvre les solutions définies.

Il faut faire un composant unique pour la gestion des acteurs. Il faut faire autant de webapp qu'il y a de type d'acteur (ou presque, Client, fournisseur, entreprise/employé)

Notre besoin : Client

__Menu d'application__

Va dans un bouton d'application. Il faut pouvoir mettre une icone pour chaque web-application.

__Second niveau__

Sur la gauche dans un menu burger.

Lorsque l'on clique sur le bouton (burger menu), on affiche la première lettre avec un fond de couleur en fonction de la première lettre.



Exemple de navigation :
-----------------------
On est sur la liste des clients, on selectionne un client, on va dans la liste des employés/contacts, on sélectionne un contact. Dans ce cas, dans la barre du haut, on affiche un fil d'ariane contenant les liens vers "liste client", "monClient", "liste contacts", "monContact".

Dans l'écran, on affiche tout en haut un résumé du client avec les informations importantes (widget présentant les données résumées de l'objet sur lequel on est, exemple : Photo acteur + nom + contacts tel et mail).

En dessous de ce résumé, on a une liste déroulante nous permettant d'accéder aux onglets des informations clients. Lorsque l'utilisateur clique sur l'onglet, on l'ajoute en onglet fixe.

Il ne peut y avoir qu'un nombre limité d'onglet fixe. Si le nombre d'onglet maximum est atteint et qu'un nouvel onglet arrive, il prend la place de l'onglet le moins utilisé.


Etape 1 : POC HTML pur !
------------------------

Test de modification en live d'un markdown !