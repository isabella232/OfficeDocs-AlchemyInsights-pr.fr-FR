---
title: Utilisation des e/s VPP Applications règle Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917494"
---
# <a name="working-with-ios-vpp-applications"></a>Utilisation des e/s Applications VPP

[Comment faire pour gérer des applications iOS achetées via un programme de volume d’achat avec Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) à en savoir plus sur les fonctionnalités, les contraintes et faites utiliser Apple en Volume d’achat et la prise en charge pour qu’il dans Microsoft Intune. 
  
 **Problèmes courants :** « J’affecté à une application VPP iOS à mes utilisateurs, mais l’installation a échoué. » 
  
- Cela peut se produire si un jeton VPP unique est utilisé sur plusieurs fournisseurs de gestion des appareils mobiles. Jetons VPP d’Apple peuvent uniquement être utilisés avec un fournisseur. Si vous avez utilisé un jeton VPP avec plusieurs fournisseurs, vous devez téléchargez de nouveau le jeton au Intune.
    
- L’installation peut également échouer si le nombre total d’installations dépasse le nombre de licences. Pour afficher un rapport d’utilisation pour vos licences, accédez à **applications Intune Mobile** \> page **licences des applications** . Pour savoir comment récupérer des licences en cours d’utilisation, voir [cet article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

