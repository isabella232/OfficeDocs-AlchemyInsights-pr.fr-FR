---
title: Utilisation de l’ID de règle des applications VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364848"
---
# <a name="working-with-ios-vpp-applications"></a>Utilisation des applications VPP iOS

Découvrez [Comment gérer les applications iOS achetées via un programme d’achat en volume avec Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) pour en savoir plus sur les fonctionnalités, les contraintes et les étapes à suivre pour utiliser le programme d’achat en volume Apple et la prise en charge de celui-ci dans Microsoft Intune.
  
 **Problèmes courants:** «J’ai affecté une application iOS VPP à mes utilisateurs, mais l’installation a échoué».
  
- Cela peut se produire si un seul jeton VPP est utilisé sur plusieurs fournisseurs de gestion des appareils mobiles. Les jetons VPP d’Apple ne peuvent être utilisés qu’avec un seul fournisseur. Si vous avez utilisé un jeton VPP avec plusieurs fournisseurs, vous devez télécharger de nouveau le jeton vers Intune.

- L’installation peut également échouer si le nombre total d’installations est supérieur au nombre de licences. Pour afficher un rapport d’utilisation pour vos licences, accédez à la page des \> **licences d’application** pour les **applications mobiles Intune** . Pour savoir comment récupérer des licences en cours d’utilisation, reportez-vous à [cet article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
