---
title: 932 AADConnect mise à niveau
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469060"
---
# <a name="upgrade-azure-ad-connect"></a>Connexion de mise à niveau Azure AD

Par défaut, mise à niveau automatique est activée pour se connecter AD Azure, qui permet de garantir vous exécutez la dernière version. Pour vérifier les paramètres de mise à niveau automatiques, utilisez l’applet de commande **Get-ADSyncAutoUpgrade** dans Windows Azure AD PowerShell. L’applet de commande renvoie une des valeurs suivantes : 
  
- **Activé**: mise à niveau automatique est activée. 
    
- **Désactivé**: mise à jour automatique est désactivée. 
    
- **Suspendu**: le système n’est plus autorisé à recevoir des mises à jour automatiques. Vous ne pouvez pas configurer cette valeur ; Il est défini par le système. 
    
Pour plus d’informations, voir [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Pour télécharger la dernière version d’Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

