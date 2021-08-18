---
title: Comment ajouter ou supprimer un délégué dans Outlook pour Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329023"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Comment ajouter ou supprimer un délégué dans Outlook pour Windows

Pour ajouter un délégué dans Outlook pour Windows : 

1. Cliquez sur **l’onglet Fichier** suivi du compte **Paramètres,** puis choisissez **Accès délégué.**
2. Cliquez sur **Ajouter.** Si **Add** n’apparaît pas, il se peut qu’il n’existe pas de connexion active entre Outlook et Exchange. La Outlook d’état affiche l’état de la connexion.
3. Tapez le nom de la personne que vous souhaitez désigner comme délégué, ou recherchez et choisissez le nom dans la liste des résultats de la recherche.

    **Remarque**: le délégué doit être une personne de la liste d’adresses globale Exchange de votre organisation.
4. Cliquez sur **Ajouter** suivi de **OK.**
5. Dans la **boîte de dialogue Déléguer des autorisations,** acceptez les paramètres d’autorisation par défaut ou sélectionnez des niveaux d’accès personnalisés pour Exchange dossiers.

    - Si un délégué a besoin d’autorisation pour travailler uniquement avec les demandes de réunion et les réponses, les paramètres d’autorisation par défaut tels que Délégué reçoivent des copies des **messages relatifs** à la réunion qui m’ont été envoyés. Vous pouvez laisser le paramètre **d’autorisation** Boîte de réception sur **Aucun**. Les demandes de réunion et les réponses sont directement dans la boîte de réception du délégué.

    **Remarque**: par défaut, le délégué se voit accorder l’autorisation Éditeur **(peut lire,** créer et modifier des éléments) pour votre **dossier** Calendrier. Lorsque le délégué répond à une réunion en votre nom, il est automatiquement ajouté à votre **dossier** Calendrier.

5. Pour envoyer un message pour informer le délégué des autorisations modifiées, cochez la case Envoyer automatiquement un message à déléguer en récapitulant ces **autorisations.**
6. Si vous le souhaitez, cochez la case **Délégué pour** mes éléments privés.

    **Important**: ce paramètre affecte tous les Exchange dossiers. Cela inclut tous les dossiers Courrier, Contacts, Calendrier, Tâches, Notes et Journal. Il n’existe aucun moyen d’accorder l’accès aux éléments privés dans les dossiers spécifiés uniquement.

7. Sélectionnez **OK**.

    **Remarque** :
    - Les messages envoyés avec des autorisations Envoyer de la part de incluent à la fois les noms du délégué et vos noms en de **côté.** Lorsqu’un message est envoyé avec les autorisations Envoyer en tant que, seul votre nom apparaît.
    - Une fois que vous avez ajouté une personne en tant que délégué, elle peut ajouter votre boîte aux lettres Exchange à son profil Outlook utilisateur. Pour obtenir des instructions, voir Gérer les éléments de courrier et [de calendrier d’une autre personne.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)

Pour supprimer un délégué dans Outlook pour Windows :

1. Cliquez sur **l’onglet** Fichier.
2. Cliquez sur **Compte Paramètres** suivi de **l’accès délégué.**
3. Choisissez le nom du délégué pour lequel vous souhaitez modifier les autorisations, puis cliquez sur Supprimer **suivi** de **OK.**
