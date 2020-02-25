---
title: Active Directory n’est pas en cours de synchronisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265193"
---
# <a name="active-directory-not-syncing"></a>Active Directory n’est pas en cours de synchronisation

Si vous recevez des erreurs de synchronisation, telles que « pas de synchronisation récente », ou Notez que l’état de synchronisation d’annuaires dans le portail d’administration Office indique « dernière synchronisation il y a plus de 3 jours », cela peut être que les paramètres de AADConnect sont incorrects ou insuffisants autorisations pour effectuer une synchronisation.  

La réinstallation de AADConnect à l’aide des paramètres rapides peut résoudre le problème rapidement :

1. [Téléchargez la dernière version de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Suivez les instructions pour l’installation d’Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Pour plus d’informations sur les comptes de service AADConnect, reportez-vous à la rubrique [Azure ad Connect : comptes et autorisations](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
