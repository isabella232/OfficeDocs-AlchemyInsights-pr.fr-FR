---
title: Corriger la stratégie de client (remplacement d’action)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326795"
---
# <a name="fix-tenant-policy-action-override"></a>Corriger la stratégie de client (remplacement d’action)

L’une de vos stratégies anti-courrier indésirable a affecté ce message. Pour passer en revue les stratégies, vous pouvez suivre les étapes suivantes :

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> , go to Email & **Collaboration** Policies \> **& Rules** Threat \> **policies** \> **Anti-spam** in the **Policies** section.

   Pour accéder directement à la page **Stratégies anti-courrier indésirable**, utilisez <https://security.microsoft.com/antispam>.

2. Dans la page Stratégies anti-courrier indésirable, sélectionnez la stratégie en cliquant sur  le nom de la stratégie ( Le **type** est Stratégie **anti-courrier** indésirable personnalisée ou Nom stratégie de courrier indésirable entrant **anti-courrier indésirable (par défaut).** 
3. Dans le volet d’informations qui s’affiche, sélectionnez **Modifier les actions** dans la section **Actions.**
4. Dans la section **Actions** de message, consultez les verdicts  pour le courrier **indésirable,** le courrier indésirable à niveau de confiance **élevé,** le hameçonnage et le hameçonnage à haut niveau de confiance pour voir si l’une des valeurs suivantes est sélectionnée :
   - **Ajouter un en-tête X**
   - **Ajouter un texte au début de la ligne d'objet**
   - **Rediriger le message vers une adresse e-mail**
   - **Supprimer le message**
   - **Aucune action**

   Il est possible que les **paramètres Standard appliqués** à tous les clients Exchange Online Protection le message.

Si vous souhaitez en savoir plus, consultez l’article [Configurer les stratégies anti-courrier indésirable dans EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
