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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937099"
---
# <a name="active-directory-not-syncing"></a>Synchronisation d’Active Directory non

Si vous recevez des erreurs de synchronisation, telles que « aucune synchronisation récente », ou si vous remarquez que l’état de synchronisation d’annuaires dans le portail d’administration Office indique « Dernière synchronisation il y a plus de 3 jours », il se peut qu’AADConnect dispose de paramètres incorrects ou d’autorisations insuffisantes pour effectuer une synchronisation.  

La réinstallation d’AADConnect à l’aide de paramètres express peut résoudre rapidement le problème :

1. [Téléchargez la dernière version d’AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Suivez les instructions pour l’installation rapide.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect doit être installé sur Windows Server 2012 ou version ultérieure. Ce serveur doit être joint au domaine et peut être un contrôleur de domaine ou un serveur membre. Pour obtenir la liste complète des conditions Connecter et des conditions préalables [d’Azure AD,](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)examinez les conditions préalables pour Azure AD Connecter .

Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
