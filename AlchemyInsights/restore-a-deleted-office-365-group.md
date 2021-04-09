---
title: Restaurer un groupe Microsoft 365 supprimé
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645129"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurer un groupe Microsoft 365 supprimé

Vous pouvez restaurer un groupe Microsoft 365 supprimé ou Microsoft Teams dans les 30 jours suivant la suppression.

1. Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of you’re the deleted groups and teams.

    **Remarque :** Connectez-vous à l’aide du compte attribué à l’administrateur client ou au rôle d’administrateur des groupes.

1. Sélectionnez le groupe Microsoft 365 supprimé/Teams à restaurer, puis cliquez sur **Restaurer le groupe.**

    Si le groupe ne peut pas être restauré en raison d’une adresse SMTP conflictuelle, utilisez la commande suivante pour rechercher l’objet à l’origine du conflit et supprimez l’adresse SMTP :

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Remarque :** Dans certains cas, la restauration du groupe et de toutes ses données peut prendre jusqu’à 24 heures.

    Pour plus d’informations ou pour découvrir comment restaurer des groupes à l’aide de PowerShell, voir Restaurer un groupe [Microsoft 365 supprimé.](https://go.microsoft.com/fwlink/?linkid=867802)