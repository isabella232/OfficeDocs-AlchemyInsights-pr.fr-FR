---
title: Synchronisation UPN désactivée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921706"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez démarré la synchronisation Azure Active Directory avant le 30 mars 2016, exécutez l’applet de commande Windows Azure AD PowerShell suivante pour activer la correspondance logicielle UPN pour seulement votre organisation :
  
 **Set-MsolDirSyncFeature-fonctionnalités EnableSoftMatchOnUpn-activer $True**
  
Correspondance logicielle UPN est automatiquement activé pour les organisations qui a démarré la synchronisation Azure AD ou après le 30 mars 2016.
  
Pour en savoir plus sur l’activation de correspondance souple sur UPN et d’autres fonctionnalités de synchronisation, voir [fonctionnalités de service de synchronisation Azure Active Directory se connecter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

