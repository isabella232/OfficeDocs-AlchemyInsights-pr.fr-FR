---
title: Utilisation de l’accès conditionnel avec Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005772"
---
# <a name="using-conditional-access-with-intune"></a>Utilisation de l’accès conditionnel avec Intune

L’utilisation de l’accès conditionnel avec Intune nécessite 3 étapes :

- [Créez une stratégie de conformité pour définir des paramètres qui doivent être respectés avant que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir une broche d’au moins 6 chiffres avant d’être considéré comme conforme.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Créez une stratégie d’accès conditionnel qui définit les ressources protégées et les conditions qui doivent être remplies pour accéder à ces ressources. Par exemple, un appareil doit être conforme avant d’accéder à la messagerie d’entreprise.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Assurez-vous que les stratégies de conformité et les stratégies d’accès conditionnel sont ciblées sur les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes spécifiques d’utilisateurs Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[En savoir plus](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
