---
title: Recherche et suppression de messages électroniques dans votre organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948881"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Recherche et suppression de messages électroniques dans votre organisation

Procédez comme suit :

1. Si vous n’êtes pas un administrateur général, pour rechercher des messages, votre compte doit être ajouté au groupe de rôles Gestionnaire **eDiscovery** ou au rôle de gestion de la recherche de **conformité.** Pour supprimer des messages, vous  devez rejoindre le groupe de rôles Gestion de l’organisation ou le rôle de gestion recherche **et purge.** Les autorisations sur ces rôles sont attribuées dans le [Centre de sécurité & conformité.](https://protection.office.com)
2. [Créez une recherche de](https://docs.microsoft.com/office365/securitycompliance/content-search) contenu pour rechercher le message à supprimer.
3. [Se connecter à l’interface PowerShell du Centre de sécurité et conformité](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Si vous utilisez l’authentification multifacteur, consultez les instructions suivantes : Connecter au Centre de sécurité & conformité PowerShell à l’aide de l’authentification [multifacteur](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Supprimez le message : exécutez `New-ComplianceSearchAction` la cmdlet pour supprimer le message. Les messages supprimés sont déplacés vers le dossier Éléments récupérables d’un utilisateur. Pour obtenir un exemple de commande, [voir Étape 3 : Supprimer le message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
