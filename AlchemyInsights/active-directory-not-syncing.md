---
title: Synchronisation d’Active Directory non
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930973"
---
# <a name="active-directory-not-syncing"></a>Synchronisation d’Active Directory non

Si vous recevez des erreurs de synchronisation, telles que « aucune synchronisation récente », ou si vous remarquez que l’état de la synchronisation d’annuaires dans le portail d’administration Office indique « Dernière synchronisation il y a plus de 3 jours », il se peut qu’AADConnect dispose de paramètres incorrects ou d’autorisations insuffisantes pour effectuer une synchronisation.  

La réinstallation d’AADConnect à l’aide de paramètres express peut résoudre rapidement le problème :

1. [Téléchargez la dernière version d’AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Suivez les instructions pour l’installation rapide.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect doit être installé sur Windows Server 2012 ou version ultérieure. Ce serveur doit être joint au domaine et peut être un contrôleur de domaine ou un serveur membre. Pour obtenir la liste complète des conditions requises et Connecter azure AD, examinez les conditions préalables pour [Azure AD Connecter](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
