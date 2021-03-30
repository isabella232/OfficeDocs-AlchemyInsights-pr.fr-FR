---
title: Configurer le point de terminaison DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402419"
---
# <a name="configure-endpoint-dlp"></a>Configurer le point de terminaison DLP

Microsoft Endpoint DLP vous permet d’étendre la protection et la fonctionnalité de surveillance de DLP aux informations sensibles sur les appareils Windows 10. Une fois que les appareils sont intégrés à la gestion des appareils, vous pouvez créer des stratégies DLP afin d’appliquer des actions de protection sur les éléments. L’Explorateur d’activités peut être utilisé pour surveiller l’activité des éléments sensibles. Pour plus d’informations, consultez [Appareils d’intégration dans la gestion des appareils](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Pour commencer à utiliser point de terminaison DLP :

- Vérifiez que vous disposez des licences SKU/abonnements appropriées. Pour plus d’informations, consultez [Licences SKU/abonnements](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Vérifiez les autorisations requises pour activer la gestion des appareils, accéder à la page d’intégration ou activer/désactiver la surveillance de l’appareil. Pour plus d’informations, consultez [Autorisations](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Intégrez des appareils dans la gestion des appareils en suivant la procédure sur les appareils d’intégration. Si vous ne disposez pas de l’option d’intégration d’appareils (préversion) sous **Paramètres** de conformité M365, confirmez que vous disposez de la licence et des autorisations appropriées mentionnées ci-dessus. Pour plus d’informations, consultez [Appareils d’intégration](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Créez des stratégies DLP pour protéger vos éléments sensibles. Pour plus d’informations [Scénarios de stratégie DLP pour les points de terminaison](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Pour plus d’informations sur le point de terminaison Microsoft DLP, consultez [En savoir plus sur les points de terminaison de protection contre la perte de données Microsoft 365 (préversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Étapes importantes de la collecte de données si une prise en charge est nécessaire :**

1. Téléchargez l'aperçu du MDATP Client Analyzer sur [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Exécutez l’outil en tant qu’administrateur à partir de la fenêtre cmd :
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Lorsque le message « Entrez le nombre de minutes pour collecter les traces » vous est demandé : entrez le nombre de minutes nécessaires pour exécuter le scénario
5. Exécuter le scénario

Collectez la sortie du fichier zip à remettre à l'agent de support.
