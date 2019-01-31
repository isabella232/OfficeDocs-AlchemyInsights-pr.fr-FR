---
title: Synchronisation UPN désactivée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657969"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez démarré la synchronisation Azure Active Directory avant le 30 mars 2016, exécutez l’applet de commande Windows Azure AD PowerShell suivante pour activer la correspondance logicielle UPN pour seulement votre organisation :
  
 **Set-MsolDirSyncFeature-fonctionnalités EnableSoftMatchOnUpn-activer $True**
  
Correspondance logicielle UPN est automatiquement activé pour les organisations qui a démarré la synchronisation Azure AD ou après le 30 mars 2016.
  
Pour en savoir plus sur l’activation de correspondance souple sur UPN et d’autres fonctionnalités de synchronisation, voir [fonctionnalités de service de synchronisation Azure Active Directory se connecter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

