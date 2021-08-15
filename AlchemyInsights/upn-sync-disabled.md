---
title: Synchronisation UPN désactivée
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038110"
---
# <a name="upn-sync-disabled"></a>Synchronisation UPN désactivée

Si vous avez commencé la synchronisation avec Azure AD avant le 30 mars 2016, exécutez l’cmdlet Azure AD PowerShell suivante pour activer la correspondance souple UPN pour votre organisation uniquement :
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
La correspondance avec le nom d’upn soft est automatiquement désactivée pour les organisations qui ont commencé à se synchroniser avec Azure AD le 30 mars 2016 ou après.
  
Pour en savoir plus sur l’activation de la correspondance souple sur UPN et d’autres fonctionnalités de synchronisation, consultez [Azure AD Connecter service de synchronisation.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

