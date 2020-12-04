---
title: Procédure d’ajout ou de suppression d’un délégué dans Outlook pour Windows
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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571837"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Procédure d’ajout ou de suppression d’un délégué dans Outlook pour Windows

Pour ajouter un délégué dans Outlook pour Windows : 

1. Cliquez sur l’onglet **fichier** , puis sur **paramètres du compte**, et choisissez **accès délégué**.
2. Cliquez sur **Ajouter**. Si **Ajouter** n’apparaît pas, il est possible qu’une connexion active n’existe pas entre Outlook et Exchange. La barre d’État Outlook affiche l’état de la connexion.
3. Tapez le nom de la personne que vous voulez désigner comme délégué, ou recherchez et choisissez le nom dans la liste des résultats de la recherche.

    > [!NOTE]
    > Le délégué doit être une personne figurant dans la liste d’adresses globale Exchange de votre organisation.
4. Cliquez sur **Ajouter** , puis sur **OK**.
5. Dans la boîte de dialogue **autorisations des délégués** , acceptez les paramètres d’autorisation par défaut ou sélectionnez des niveaux d’accès personnalisés pour les dossiers Exchange.

    - Si un délégué a besoin de l’autorisation pour fonctionner uniquement avec des demandes de réunion et des réponses, les paramètres d’autorisation par défaut, tels que **Delegate, reçoivent une copie des messages relatifs à la réunion qui me** sont suffisants. Vous pouvez laisser le paramètre autorisation de **boîte de réception** en **aucun**. Les demandes de réunion et les réponses seront directement envoyées vers la boîte de réception du délégué.

    > [!NOTE]
    > Par défaut, l’éditeur bénéficie de l’autorisation **éditeur (peut lire, créer et modifier des éléments)** sur votre dossier **calendrier** . Lorsque le délégué répond à une réunion de votre part, il est automatiquement ajouté à votre dossier de **calendrier** .

5. Pour envoyer un message afin d’informer le délégué des autorisations modifiées, activez la case à cocher **Envoyer automatiquement un message au délégué pour résumer ces autorisations** .
6. Si vous le souhaitez, activez la case à cocher le **délégué peut voir mes éléments privés** .

    > [!IMPORTANT]
    > Ce paramètre affecte tous les dossiers Exchange. Cela inclut tous les dossiers courrier, contacts, calendrier, tâches, notes et journal. Il n’existe aucun moyen d’accorder l’accès aux éléments privés dans les dossiers spécifiés uniquement.

7. Sélectionnez **OK**.

    > [!NOTE]
    >
    > - Les messages envoyés avec les autorisations Envoyer de la part de incluent les délégués et vos noms en regard **de**. Lorsqu’un message est envoyé avec les autorisations Envoyer en tant que, seul votre nom s’affiche.
    > - Une fois que vous avez ajouté un utilisateur en tant que délégué, il peut ajouter votre boîte aux lettres Exchange à son profil Outlook. Pour obtenir des instructions, consultez [la rubrique gérer les éléments de courrier et de calendrier d’une autre personne](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Pour supprimer un délégué dans Outlook pour Windows :

1. Cliquez sur l’onglet **fichier** .
2. Cliquez sur **paramètres du compte** , puis sur **accès délégué**.
3. Sélectionnez le nom du délégué pour lequel vous souhaitez modifier les autorisations, puis cliquez sur **supprimer** suivi de **OK**.
