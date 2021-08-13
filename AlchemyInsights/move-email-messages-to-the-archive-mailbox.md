---
title: Déplacer des messages électroniques vers la boîte aux lettres d’archivage
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974955"
---
# <a name="move-email-to-the-archive-mailbox"></a>Déplacer le courrier électronique vers la boîte aux lettres d’archivage

Si vous souhaitez que nous 2007-2016 exécutez des vérifications automatisées pour les paramètres mentionnés ci-dessous, sélectionnez le bouton Retour <- en haut de cette page, puis entrez l’adresse e-mail de l’utilisateur qui a des difficultés à déplacer le courrier vers sa boîte aux lettres d’archivage.

1. Confirmez **qu’une boîte aux lettres** d’archivage a été activée. Si ce n’est pas le cas, utilisez les étapes [de cet article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) pour activer la boîte aux lettres d’archivage.

2. Pour archiver les messages automatiquement dans la boîte aux lettres d’archivage, une balise de rétention avec l’action Déplacer vers **l’archive** doit être définie pour être appliquée automatiquement à la balise de boîte aux lettres entière **(par défaut).** Utilisez les étapes ci-après pour créer la balise : [Archiver la balise par défaut.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Ensuite, ajoutez la **balise Archive** à votre stratégie de rétention. Dans le centre Exchange' administration, sélectionnez Stratégies  de **rétention** > ajouter la balise Déplacer vers l’archive à la stratégie > **Enregistrer.**

4. Maintenant, [affectez la stratégie de](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) rétention à la boîte aux lettres de l’utilisateur spécifique. La même stratégie sera appliquée à la boîte aux lettres **principale** et à la boîte **aux lettres d’archivage.**

Il peut être nécessaire de forcer l’Assistant Dossier géré (MFA) à s’exécuter et à appliquer les nouveaux paramètres à la boîte aux lettres de l’utilisateur. Exécutez la commande suivante lorsque vous [êtes connecté à EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pour démarrer l’Assistant Dossier géré pour une boîte aux lettres spécifique :
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Pour plus d’informations sur la configuration d’une stratégie d’archivage, voir Configurer une stratégie [d’archivage](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)et de suppression pour les boîtes aux lettres.
  