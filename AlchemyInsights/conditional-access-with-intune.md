---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807657"
---
# <a name="conditional-access-with-intune"></a>Accès conditionnel avec Intune

L’utilisation de l'  **accès conditionnel**  avec Intune nécessite 3 étapes :

- Créez une  **stratégie de conformité**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pour définir les paramètres qui doivent être satisfaits pour que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir un code confidentiel d’au moins 6 chiffres avant d’être considéré comme conforme.
- Créer une **stratégie d’accès conditionnel**  qui définit les ressources à protéger et les conditions à respecter pour accéder à ces ressources.  [Par exemple,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un appareil doit être conforme avant d’accéder à la messagerie d’entreprise.
- Assurez-vous que les stratégies de **conformité**  et les  **stratégies d’accès conditionnel**  sont ciblées pour les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory.

**Liens utiles :**

[Présentation de la conformité des appareils](https://docs.microsoft.com/intune/device-compliance-get-started)

[Dépannage de l’autorité de certification](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Stratégie de résolution des problèmes](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Pour protéger les messages électroniques (Exchange Online) contre les accès par des appareils non conformes, les deux documents doivent être suivis :

1. [Protection de l’accès au courrier électronique à partir d’appareils utilisant EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protéger l’accès à la messagerie des appareils utilisant des clients d’authentification modernes comme Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)