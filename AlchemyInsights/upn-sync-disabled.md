---
title: Synchronisation UPN désactivée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749512"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez commencé la synchronisation avec Azure AD avant le 30 mars 2016, exécutez l’applet de commande Azure AD PowerShell suivante pour activer la correspondance logicielle UPN pour votre organisation uniquement :
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-Enable $True**
  
La correspondance logicielle UPN est activée automatiquement pour les organisations qui ont commencé la synchronisation avec Azure AD depuis le 30 mars 2016.
  
Pour en savoir plus sur l’activation de la correspondance floue sur l’UPN et d’autres fonctionnalités de synchronisation, reportez-vous à [Azure ad Connect Sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

