---
title: Utilisation de l’ID de règle des applications VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083012"
---
# <a name="working-with-ios-vpp-applications"></a>Utilisation des applications VPP iOS

Lisez comment gérer les applications [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) achetées dans le cadre d’un programme d’achat en volume avec Microsoft Intune pour en savoir plus sur les fonctionnalités, les contraintes et les étapes à suivre pour utiliser le programme d’achat en volume Apple et sa prise en charge dans Microsoft Intune.
  
 **Problèmes courants :** « J’ai affecté une application VPP iOS à mes utilisateurs, mais l’installation a échoué. »
  
- Cela peut se produire si un jeton VPP unique est utilisé dans plusieurs fournisseurs de gestion d’appareils mobiles. Les jetons VPP d’Apple ne peuvent être utilisés qu’avec un seul fournisseur. Si vous avez utilisé un jeton VPP avec plusieurs fournisseurs, vous devez télécharger à nouveau le jeton dans Intune.

- L’installation peut également échouer si le nombre total d’installations dépasse le nombre de licences. Pour afficher un rapport d’utilisation pour vos licences, consultez la page Licences d’application des applications **Intune** \>  Mobile. Pour savoir comment récupérer les licences en cours d’utilisation, consultez [cet article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
