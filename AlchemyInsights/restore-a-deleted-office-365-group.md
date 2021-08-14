---
title: Restaurer un groupe de Microsoft 365 supprimé
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959024"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurer un groupe de Microsoft 365 supprimé

Vous pouvez restaurer un groupe Microsoft 365 supprimé ou Microsoft Teams dans les 30 jours suivant la suppression.

1. Go to the [Centre d’administration Microsoft 365](https://aka.ms/RestoreDeletedGroup) to log in to a list of you’re the deleted groups and teams.

    **Remarque :** Connectez-vous à l’aide du compte attribué à l’administrateur client ou au rôle d’administrateur des groupes.

1. Sélectionnez le groupe de Microsoft 365/Teams supprimé à restaurer, puis cliquez sur **Restaurer le groupe.**

    Si le groupe ne peut pas être restauré en raison d’une adresse SMTP conflictuelle, utilisez la commande suivante pour rechercher l’objet à l’origine du conflit et supprimez l’adresse SMTP :

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Remarque :** Dans certains cas, la restauration du groupe et de toutes ses données peut prendre jusqu’à 24 heures.

    Pour plus d’informations ou pour découvrir comment restaurer des groupes à l’aide de PowerShell, voir Restaurer un groupe [Microsoft 365 supprimé.](https://go.microsoft.com/fwlink/?linkid=867802)