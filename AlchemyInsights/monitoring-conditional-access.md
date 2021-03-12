---
title: Surveillance de l’accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708672"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Surveillance de l’accès conditionnel pour Exchange

Les utilisateurs ciblés avec un accès conditionnel recevront un e-mail de notification s’ils ne répondent pas aux exigences d’accès de votre organisation. Pour résoudre ce problème, nous vous recommandons d’apporter une ou plusieurs des solutions suivantes :

- Si l’appareil est supposé être inscrit, conseillez à l’utilisateur d’utiliser l’application Portail d’entreprise et de vérifier qu’elle apparaît dans le portail d’entreprise. Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.
- Dans le portail Azure, allez sur Intune > conformité de l’appareil. Sous Surveiller, cliquez sur Conformité de l’appareil. Affichez le rapport de conformité de votre appareil pour vérifier que l’appareil de l’utilisateur est marqué comme conforme.
- Dans le portail Azure, allez sur Intune > conformité de l’appareil. Sous Gérer, cliquez sur Stratégies. Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur. Si aucun profil n’est affecté, Intune ne sera pas en mesure de confirmer l’état de conformité de l’appareil.
- Modifiez l’affectation d’accès conditionnel de l’utilisateur.

1. Dans le portail Azure, accédez à **Stratégies d’accès**  >  **conditionnel** Intune.  >  
2. Sélectionnez une stratégie dans la liste.
3. Cliquez sur Utilisateurs et groupes.
4. Pour cibler une stratégie à une personne, ajoutez-la à la liste Inclure. Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la liste Exclure.

Liens utiles :

[Vue d’ensemble de la conformité des appareils](https://docs.microsoft.com/intune/device-compliance-get-started)

[Dépannage de l’ac](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Stratégie de dépannage](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Surveillance de la conformité des appareils Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Remarque : ces étapes sont uniquement utiles pour résoudre les problèmes d’accès conditionnel à la fonctionnalité Azure Active Directory. Il est également possible de mettre en quarantaine un appareil qui bloque son accès à la messagerie avec la stratégie Exchange. Pour plus d’informations sur la gestion des appareils Exchange, voir [ici]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
