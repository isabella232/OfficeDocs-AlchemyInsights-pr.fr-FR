---
title: Corriger la stratégie de filtrage de langue/IP
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
- "9000760"
- "7391"
ms.openlocfilehash: 16aa12120034e1f848e62bab151d8e30b251a29e5727f085300d74ca7b49ca52
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896153"
---
# <a name="fix-languageip-filter-policy"></a>Corriger la stratégie de filtrage de langue/IP

L’une de vos stratégies anti-courrier indésirable a affecté ce message. Pour passer en revue les stratégies, vous pouvez suivre les étapes suivantes :

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> , go to Email & **Collaboration** Policies \> **& Rules** Threat \> **policies** \> **Anti-spam** in the **Policies** section.

   Pour accéder directement à la page **Stratégies anti-courrier indésirable**, utilisez <https://security.microsoft.com/antispam>.

2. Dans la page Stratégies anti-courrier indésirable, sélectionnez la stratégie en cliquant sur  le nom de la stratégie ( Le **type** est Stratégie **anti-courrier** indésirable personnalisée ou Nom stratégie de courrier indésirable entrant  **(par défaut)**).
3. Dans le volet d’informations  qui s’affiche, sélectionnez Modifier le seuil de courrier indésirable et les propriétés dans la section Modifier le seuil de courrier indésirable **& propriétés du** courrier indésirable.
4. Dans la section **Marquer comme courrier indésirable,** examinez les paramètres Contient des **langues spécifiques** et **De ces pays.**

Si vous souhaitez en savoir plus, consultez l’article [Configurer les stratégies anti-courrier indésirable dans EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
