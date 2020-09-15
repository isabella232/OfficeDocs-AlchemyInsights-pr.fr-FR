---
title: Active Directory n’est pas en cours de synchronisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697627"
---
# <a name="active-directory-not-syncing"></a>Active Directory n’est pas en cours de synchronisation

Si vous recevez des erreurs de synchronisation, telles que « pas de synchronisation récente », ou Notez que l’état de synchronisation d’annuaires dans le portail d’administration Office indique « dernière synchronisation il y a plus de 3 jours », il se peut que AADConnect ait des paramètres incorrects ou des autorisations insuffisantes pour effectuer une synchronisation.  

La réinstallation de AADConnect à l’aide des paramètres rapides peut résoudre le problème rapidement :

1. [Téléchargez la dernière version de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Suivez les instructions pour l’installation d’Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
