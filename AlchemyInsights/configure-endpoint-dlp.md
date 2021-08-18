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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323916"
---
# <a name="configure-endpoint-dlp"></a>Configurer le point de terminaison DLP

Microsoft Endpoint DLP vous permet d’étendre la protection et la fonctionnalité de surveillance de DLP aux informations sensibles sur les appareils Windows 10. Une fois que les appareils sont intégrés à la gestion des appareils, vous pouvez créer des stratégies DLP afin d’appliquer des actions de protection sur les éléments. L’Explorateur d’activités peut être utilisé pour surveiller l’activité des éléments sensibles. Pour plus d’informations, consultez [Appareils d’intégration dans la gestion des appareils](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Pour commencer à utiliser point de terminaison DLP :

- Vérifiez que vous disposez des licences SKU/abonnements appropriées. Pour plus d’informations, consultez [Licences SKU/abonnements](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Vérifiez les autorisations requises pour activer la gestion des appareils, accéder à la page d’intégration ou activer/désactiver la surveillance du périphérique. Pour en savoir plus, voir [Autorisations d’accès](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Intégrez des appareils dans la gestion des appareils en suivant la procédure sur les appareils d’intégration. Pour plus d’informations, consultez [Appareils d’intégration](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Créez des stratégies DLP pour protéger vos éléments sensibles. Pour plus d’informations [Scénarios de stratégie DLP pour les points de terminaison](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Pour plus d’informations sur le point de terminaison Microsoft DLP, consultez [En savoir plus sur les points de terminaison de protection contre la perte de données Microsoft 365 (préversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Étapes importantes de la collecte de données si une prise en charge est nécessaire :**

1. Téléchargez [La version préliminaire de l’analyseur de client MDATP](https://aka.ms/betamdatpanalyzer).
1. Exécutez l’outil en tant qu’administrateur à partir de la fenêtre cmd :

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Lorsque vous êtes invité par cette note **Entrez le nombre de minutes pour collecter les traces**, entrez le nombre de minutes nécessaires pour exécuter le scénario.
1. Exécuter le scénario.

Collectez la sortie du fichier zip à remettre à l'agent de support.
