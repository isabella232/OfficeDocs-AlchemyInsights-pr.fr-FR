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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767225"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez commencé la synchronisation avec Azure AD avant le 30 mars 2016, exécutez l'applet de commande Azure AD PowerShell suivante pour activer la correspondance logicielle UPN pour votre organisation uniquement:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
La correspondance logicielle UPN est activée automatiquement pour les organisations qui ont commencé la synchronisation avec Azure AD depuis le 30 mars 2016.
  
Pour en savoir plus sur l'activation de la correspondance floue sur l'UPN et d'autres fonctionnalités de synchronisation, reportez-vous à [Azure ad Connect Sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

