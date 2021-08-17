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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889216"
---
# <a name="active-directory-not-syncing"></a>Synchronisation d’Active Directory non

Si vous recevez des erreurs de synchronisation, telles que « aucune synchronisation récente », ou si vous remarquez que l’état de synchronisation d’annuaires dans le portail d’administration Office indique « Dernière synchronisation il y a plus de 3 jours », il se peut qu’AADConnect dispose de paramètres incorrects ou d’autorisations insuffisantes pour effectuer une synchronisation.  

La réinstallation d’AADConnect à l’aide de paramètres express peut résoudre rapidement le problème :

1. [Téléchargez la dernière version d’AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Suivez les instructions pour l’installation rapide.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect doit être installé sur Windows Server 2012 ou version ultérieure. Ce serveur doit être joint au domaine et peut être un contrôleur de domaine ou un serveur membre. Pour obtenir la liste complète des conditions Connecter et des conditions préalables [d’Azure AD,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)examinez les conditions préalables pour Azure AD Connecter .

Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
