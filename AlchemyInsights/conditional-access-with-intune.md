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
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069710"
---
# <a name="conditional-access-with-intune"></a>Accès conditionnel avec Intune

**L’utilisation de l’accès** conditionnel avec Intune nécessite 3 étapes :

- Créez **une stratégie de** conformité ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pour définir les paramètres qui doivent être respectés avant que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir une broche d’au moins 6 chiffres avant d’être considéré comme conforme.
- Créez **une stratégie d’accès**  conditionnel qui définit les ressources protégées et les conditions qui doivent être remplies pour accéder à ces ressources.  [Par exemple, un](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  appareil doit être conforme avant d’accéder à la messagerie d’entreprise.
- Assurez-vous **que les stratégies de**  conformité et les  **stratégies**  d’accès conditionnel sont ciblées sur les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes spécifiques d’utilisateurs Azure Active Directory.

**Liens utiles :**

[Vue d’ensemble de la conformité des appareils](https://docs.microsoft.com/intune/device-compliance-get-started)

[Dépannage de l’ac](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Stratégie de dépannage](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Pour protéger la messagerie (Exchange en ligne) contre l’accès par des appareils non conformes, les deux documents doivent être suivis :

1. [Protéger l’accès à la messagerie à partir d’appareils à l’aide d’EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protéger l’accès à la messagerie à partir d’appareils utilisant des clients d’authentification modernes tels que Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)