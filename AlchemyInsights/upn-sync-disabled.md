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
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288816"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez démarré la synchronisation Azure Active Directory avant le 30 mars 2016, exécutez l’applet de commande Windows Azure AD PowerShell suivante pour activer la correspondance logicielle UPN pour seulement votre organisation :
  
 **Set-MsolDirSyncFeature-fonctionnalités EnableSoftMatchOnUpn-activer $True**
  
Correspondance logicielle UPN est automatiquement activé pour les organisations qui a démarré la synchronisation Azure AD ou après le 30 mars 2016.
  
Pour en savoir plus sur l’activation de correspondance souple sur UPN et d’autres fonctionnalités de synchronisation, voir [fonctionnalités de service de synchronisation Azure Active Directory se connecter](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

