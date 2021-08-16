---
title: Surveiller l’accès conditionnel à Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025500"
---
# <a name="monitor-intune-conditional-access"></a>Surveiller l’accès conditionnel à Intune

Les utilisateurs ciblés avec un accès conditionnel recevront un e-mail de notification s’ils ne répondent pas aux exigences d’accès de votre organisation. Pour résoudre ce problème, nous vous recommandons d’apporter une ou plusieurs des solutions suivantes :

1. Si l’appareil est supposé être inscrit, conseillez à l’utilisateur d’utiliser l’application Portail d’entreprise et de vérifier qu’elle apparaît dans le Portail d’entreprise. Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.
1. Dans le portail Azure, allez à la conformité **des appareils Intune.**  >   
1. Pour afficher le rapport de conformité de votre appareil afin de vérifier que l’appareil de l’utilisateur est marqué comme conforme, sous **Surveiller,** cliquez sur **Conformité de l’appareil.**
1. Dans le portail Azure, allez à la conformité **des appareils Intune.**  >   Sous **Gérer, cliquez** sur **Stratégies.** Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur. Si aucun profil n’est affecté, Intune ne sera pas en mesure de confirmer l’état de conformité de l’appareil.
1. Modifier l’affectation d’accès conditionnel de l’utilisateur.
1. Dans le portail Azure, accédez à Stratégies d’accès conditionnel **Intune,** sélectionnez une stratégie dans la liste, puis cliquez sur Utilisateurs  >    >   **et groupes.**
1. Pour cibler une stratégie à quelqu’un, ajoutez-la à la **liste Inclure.** Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la **liste Exclure.**

**Liens utiles :**

- [Vue d’ensemble de la conformité des appareils](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Dépannage de l’ac](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Stratégie de dépannage](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Surveillance de la conformité des appareils Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ces étapes ne sont utiles que dans le dépannage de la fonctionnalité Azure Active Directory’accès conditionnel. Il est également possible de mettre en quarantaine un appareil qui bloque son accès à la messagerie avec Exchange stratégie. Pour plus d’informations Exchange gestion des appareils, voir [**ici.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
