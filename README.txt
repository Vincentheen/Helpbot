SCP-Reloaded - Guide Complet du Bot Discord
===========================================

Table des matières
-----------------
1. Introduction
2. Premiers pas
3. Commandes Générales
4. Système de Tickets
5. Système de Modération
6. Système de Règlement
7. Gestion des Rôles
8. Système de Giveaway
9. Dépannage
10. FAQ

Introduction
-----------

SCP-Reloaded est un bot Discord multifonction conçu pour faciliter la gestion de votre serveur. Il offre de nombreuses fonctionnalités comme un système de tickets, un système de modération, un système de règlement, et bien plus encore.

Ce guide vous expliquera en détail comment utiliser toutes les fonctionnalités du bot, des commandes de base aux fonctionnalités les plus avancées.

Premiers pas
-----------

Prérequis:
- Un serveur Discord
- Les permissions administrateur sur ce serveur

Configuration initiale:
1. Le bot a déjà été ajouté à votre serveur par votre fournisseur
2. Utilisez la commande !checksetup pour vérifier si le serveur est correctement configuré
3. Configurez les rôles de staff avec les commandes suivantes :
   - !setownerrole @role - Définit le rôle propriétaire du serveur
   - !setadminrole @role - Définit le rôle administrateur
   - !setmodrole @role - Définit le rôle modérateur
   - !sethelperrole @role - Définit le rôle helper

Vérification de la configuration:
Utilisez la commande !checksetup à tout moment pour vérifier si votre serveur est correctement configuré. Le bot vous indiquera les éléments manquants ou mal configurés.

Commandes Générales
------------------

Commandes de base:
- !hello - Le bot répond avec un message sympa
- !commands ou !cmdlist - Affiche la liste des commandes disponibles
- !serverinfo - Affiche les informations du serveur
- !userinfo [@utilisateur] - Affiche les informations d'un utilisateur
- !avatar [@utilisateur] - Affiche l'avatar d'un utilisateur

Configuration du serveur:
- !checksetup - Vérifie si le serveur est correctement configuré
- !setjoinleavechannel [#canal] - Configure le canal pour les logs d'arrivées et départs

Système de Tickets
-----------------

Le système de tickets permet aux utilisateurs de créer des tickets pour contacter le staff du serveur. Les tickets sont organisés par catégories pour faciliter leur gestion.

Configuration du système de tickets:
- !setupticketsfr - Configure le système de tickets avec les catégories en français
- !checksetupfr - Vérifie si les catégories en français sont correctement configurées

Catégories de tickets en français:
1. 📋 Recrutement Staff
2. 💼 Recrutement Entreprise
3. 🎮 Support Jeu
4. 🔨 Contestation Sanction
5. 📢 Signalement

Commandes de gestion des tickets:
- !ticket - Crée un message avec les boutons de création de ticket
- !resetticket - Recréer le message de ticket dans le canal ticket-support
- !renameticket <nouveau_nom> - Renomme un ticket
- !addmember @utilisateur - Ajoute un membre au ticket
- !removemember @utilisateur - Retire un membre du ticket
- !listtickets - Affiche la liste des tickets actifs

Fonctionnement des tickets:
1. Un utilisateur clique sur un bouton correspondant à la catégorie de son ticket
2. Un canal de ticket est créé avec le nom de l'utilisateur (ex: ticket-username-1)
3. L'utilisateur peut discuter avec le staff dans ce canal
4. Le ticket peut être fermé, supprimé ou rouvert à l'aide des boutons

Boutons de gestion des tickets:
- Fermer le ticket - Ferme le ticket (personne ne peut plus y écrire)
- Supprimer le ticket - Supprime définitivement le canal du ticket
- Rouvrir le ticket - Rouvre un ticket fermé

Système de Modération
--------------------

Le système de modération permet aux membres du staff de gérer les utilisateurs du serveur, de sanctionner les comportements inappropriés et de maintenir l'ordre.

Commandes de modération:
- !ban @utilisateur [raison] - Bannir un utilisateur
- !unban ID_utilisateur - Débannir un utilisateur
- !kick @utilisateur [raison] - Expulser un utilisateur
- !mute @utilisateur [durée] [raison] - Rendre muet un utilisateur
- !unmute @utilisateur - Rendre la parole à un utilisateur
- !clear [nombre] - Supprimer des messages
- !warn @utilisateur [raison] - Avertir un utilisateur
- !warnings @utilisateur - Voir les avertissements d'un utilisateur
- !clearwarns @utilisateur - Effacer les avertissements d'un utilisateur

Filtrage des mots:
- !addword <mot> - Ajouter un mot à la liste des mots interdits
- !removeword <mot> - Retirer un mot de la liste des mots interdits
- !listwords - Afficher la liste des mots interdits

Annonces:
- !annonce <message> - Envoyer une annonce formatée
- !say <message> - Faire parler le bot
- !saytitle <titre> <message> - Faire parler le bot avec un titre et un message

Système de Règlement
-------------------

Le système de règlement permet de créer et gérer un règlement pour votre serveur, avec un système de vérification pour les nouveaux membres.

Configuration du règlement:
- !setupreglement [#canal] - Configurer le canal de règlement
- !addrule <texte> - Ajouter une règle au règlement
- !removerule <numéro> - Supprimer une règle du règlement
- !editrule <numéro> <texte> - Modifier une règle existante
- !showrules - Afficher la liste des règles
- !setbanner [url] - Changer la bannière du règlement
- !resetrules - Supprimer toutes les règles

Système de vérification:
- !showrules - Afficher le règlement avec un bouton pour accepter et obtenir le rôle membre

Gestion des Rôles
----------------

Le système de gestion des rôles permet de créer, configurer et attribuer des rôles aux membres du serveur.

Configuration des rôles:
- !createrole <nom> <couleur> commandes... - Crée un nouveau rôle Discord
- !setrole <nom> <@role ou nom> commandes... - Configure un rôle existant
- !listroles - Affiche tous les rôles configurés
- !delrole <nom ou @mention> - Supprime un rôle Discord du serveur

Gestion des permissions:
- !addrolecommand <nom ou @mention> commandes... - Ajoute des commandes à un rôle
- !removerolecommand <nom ou @mention> commandes... - Retire des commandes d'un rôle
- !staffperms [owner/admin/mod/helper] - Affiche les permissions détaillées du staff
- !permissions [nom ou @mention] - Affiche les permissions d'un rôle
- !perms [nom ou @mention] - Alias de permissions
- !addperm <nom ou @mention> <commande> - Ajoute une permission à un rôle
- !removeperm <nom ou @mention> <commande> - Retire une permission d'un rôle
- !resetperms [mod/helper/all] - Réinitialise les permissions

Attribution des rôles:
- !addrole @utilisateur @rôle - Ajouter un rôle à un utilisateur
- !removerole @utilisateur @rôle - Retirer un rôle à un utilisateur

Système de Giveaway
------------------

Le système de giveaway permet d'organiser des concours sur votre serveur.

Commandes de giveaway:
- !giveaway <durée_en_secondes> <prix> - Crée un giveaway basé sur le temps
- !giveaway m:<nombre_membres> <prix> - Crée un giveaway qui se termine quand le serveur atteint un certain nombre de membres
- !endgiveaway - Termine immédiatement le giveaway en cours et choisit un gagnant
- !stopgiveaway - Arrête le giveaway en cours sans choisir de gagnant

Dépannage
---------

Problèmes courants et solutions:

Le bot ne répond pas aux commandes:
1. Vérifiez que le bot est en ligne
2. Vérifiez que vous avez les permissions nécessaires pour utiliser la commande
3. Vérifiez que la commande est correctement écrite

Les tickets ne fonctionnent pas correctement:
1. Utilisez !checksetupfr pour vérifier si les catégories sont correctement configurées
2. Utilisez !setupticketsfr pour reconfigurer le système de tickets
3. Vérifiez que le bot a les permissions nécessaires dans les catégories de tickets

Les rôles ne sont pas attribués correctement:
1. Vérifiez que le bot a la permission de gérer les rôles
2. Vérifiez que le rôle du bot est placé au-dessus des rôles qu'il doit attribuer dans la hiérarchie des rôles

Comment signaler un bug:
Si vous rencontrez un bug qui n'est pas mentionné ici, veuillez contacter l'administrateur du bot avec les informations suivantes :
1. Description détaillée du problème
2. Étapes pour reproduire le bug
3. Captures d'écran si possible

FAQ
---

Questions générales:

Q: Comment inviter le bot sur mon serveur ?
R: Contactez l'administrateur du bot pour obtenir un lien d'invitation.

Q: Le bot est-il gratuit ?
R: Oui, le bot est entièrement gratuit à utiliser.

Q: Puis-je modifier le bot ?
R: Le code source du bot est disponible, mais toute modification doit être faite par un développeur qualifié.

Questions sur les tickets:

Q: Comment créer un ticket ?
R: Cliquez sur l'un des boutons dans le message de création de ticket.

Q: Comment fermer un ticket ?
R: Cliquez sur le bouton "Fermer le ticket" dans le canal du ticket.

Q: Comment supprimer un ticket ?
R: Après avoir fermé un ticket, cliquez sur le bouton "Supprimer le ticket".

Questions sur la modération:

Q: Comment bannir un utilisateur ?
R: Utilisez la commande !ban @utilisateur [raison].

Q: Comment voir les avertissements d'un utilisateur ?
R: Utilisez la commande !warnings @utilisateur.

Q: Comment supprimer plusieurs messages à la fois ?
R: Utilisez la commande !clear [nombre].

---

Crédits et Remerciements

SCP-Reloaded a été développé par l'équipe de développement SCP-Reloaded.

Pour toute question ou suggestion, veuillez contacter l'administrateur du bot.

---

Ce guide est susceptible d'être mis à jour. Dernière mise à jour : 10/04/2025