---
title: Les indicateurs ne fonctionnent pas à l’aide du navigateur Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887438"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Les indicateurs ne fonctionnent pas à l’aide du navigateur Edge

Une fois que vous avez créé un indicateur, il n'est pas reconnu par Edge (Smartscreen). Pour plus d’informations, consultez [Créer des indicateurs pour les IP et URL/domaines](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Étape 1 : vérifier les éléments suivants

- Vérifiez que l’indicateur est correct (aucune faute de frappe dans IP/URL, action correcte, groupes RBAC corrects).
- Attendez au minimum 2 heures après la création de l'indicateur pour tenir compte d'une éventuelle latence.
- Confirmez que le ou les systèmes sont intégrés à Microsoft Defender pour point de terminaison.
- Vérifiez que le ou les systèmes peuvent communiquer avec le cloud.
- Vérifiez que Smartscreen est activé et accessible en accédant au [site de test](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Étape 2 : résoudre le problème potentiel

- Assurez-vous que le client répond aux exigences. Pour plus d’informations, consultez [Créer des indicateurs pour les IP et URL/domaines](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Assurez-vous que vous exécutez la dernière version du navigateur Edge. Pour connaître la dernière version, consultez [Découvrez la version de Microsoft Edge que vous avez](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Redémarrez le navigateur Edge.
- Accédez au site pour lequel vous avez configuré un indicateur. Si le site n’apparaît pas comme prévu, passez à l’étape 3. 

## <a name="step-3-collect-data"></a>Étape 3 : collecter les données

- Collectez les données de diagnostic **MDEClientAnalyzer**. Pour obtenir des instructions, consultez [Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison](issues-with-onboarding-machines.md).
- Si vous êtes à l’aise avec l’installation et la collecte d’une trace Fiddler, consultez [Telerik Fiddler](http://www.telerik.com/fiddler).
- Si vous préférez obtenir des conseils à partir de Support Microsoft, sélectionnez l’icône Support ci-dessous pour ouvrir un cas de support.
