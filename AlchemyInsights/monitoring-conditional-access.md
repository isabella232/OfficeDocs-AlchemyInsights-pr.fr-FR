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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366426"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Surveillance de l’accès conditionnel pour Exchange

Les utilisateurs ciblés avec l’accès conditionnel recevront un courrier électronique de notification s’ils ne répondent pas aux exigences d’accès de votre organisation. Pour résoudre ce qui suit, nous vous recommandons d’utiliser une ou plusieurs des solutions suivantes :

- Si le périphérique est présumé être inscrire, conseillez-lui d’accéder à l’application portail d’entreprise et de vérifier qu’il apparaît dans le portail d’entreprise. Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.
- Dans le portail Azure, accédez à Intune > la conformité des appareils. Sous analyse, cliquez sur conformité des appareils. Affichez votre rapport de conformité des appareils pour vérifier que l’appareil de l’utilisateur est marqué comme étant compatible.
- Dans le portail Azure, accédez à Intune > la conformité des appareils. Sous gérer, cliquez sur stratégies. Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur. Si aucun profil n’est affecté, Intune ne pourra pas confirmer l’état de conformité de l’appareil.
- Modifiez l’attribution d’accès conditionnel de l’utilisateur.

1. Dans le portail Azure, accédez **Intune**aux stratégies d'  >  **accès conditionnel**Intune  >  **Policies**.
2. Sélectionnez une stratégie dans la liste.
3. Cliquez sur utilisateurs et groupes.
4. Pour cibler une stratégie spécifique à une personne, ajoutez-la à la liste inclure. Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la liste d’exclusion.

Liens utiles :

[Présentation de la conformité des appareils](https://docs.microsoft.com/intune/device-compliance-get-started)

[Dépannage de l’autorité de certification](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Stratégie de résolution des problèmes](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Surveillance de la conformité des appareils Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Remarque : ces étapes ne sont utiles que pour résoudre les problèmes liés à l’accès conditionnel à la fonctionnalité Azure Active Directory. Il est également possible de mettre en quarantaine un appareil qui bloque l’accès à la messagerie avec la stratégie Exchange. Vous trouverez plus d’informations sur la gestion des appareils Exchange [ici](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
