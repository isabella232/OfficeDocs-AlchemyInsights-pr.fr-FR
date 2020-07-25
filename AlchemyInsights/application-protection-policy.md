---
title: Stratégie de protection des applications
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266434"
---
# <a name="application-protection-policy"></a>Stratégie de protection des applications

Si vous débutez sur la stratégie de protection des applications, consultez la [Vue d’ensemble des stratégies de protection des applications](https://docs.microsoft.com/intune/apps/app-protection-policy).

Pour commencer à utiliser l’application, consultez [Guide pratique de gestion et affectation des stratégies de protection des applications](https://docs.microsoft.com/intune/app-protection-policies).

Configuration requise pour la stratégie de protection des applications :

- Un utilisateur a une licence Intune ou EMS.
- L’utilisateur appartient à un groupe ciblé par les stratégies de protection des applications.
- Un seul utilisateur d’entreprise est connecté aux applications protégées sur un appareil.
- L’application a implémenté le [Kit de développement logiciel de Intune](https://docs.microsoft.com/intune/app-sdk-get-started). Pour obtenir la liste des applications qui prennent en charge le SDK, consultez [Applications protégées Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Les stratégies s’appliquent une fois qu’un utilisateur répondant aux conditions ci-dessus se connecte à une application Intune du kit de développement logiciel compatible. La façon la plus simple de déterminer si une stratégie est appliquée est d’exiger que l’utilisateur définisse un code confidentiel dans la stratégie. 

Pour plus d’informations, voir :

[Forum aux questions sur l’application/GAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Valider la configuration de votre stratégie de protection des applications](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Comprendre le minutage de la remise des stratégies de protection des applications](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Comment surveiller les stratégies de protection des applications](https://docs.microsoft.com/intune/app-protection-policies-monitor)