---
title: Résoudre les problèmes courants liés à Microsoft Defender pour Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330058"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Résoudre les problèmes courants liés à Microsoft Defender pour Office 365

Voici quelques solutions aux problèmes courants liés à Microsoft Defender pour Office 365 :

- **Délai du message**:

  Les retards de remise du courrier électronique peuvent être dus Coffre’analyse des pièces jointes des messages. Pour plus d’informations, [Coffre paramètres de stratégie pièces jointes.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Signalez les résultats faux positifs ou négatifs**:

  Pour plus d’informations, voir [Signaler des messages et des fichiers à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Activez Coffre protection des liens**:

  1. Dans le portail Microsoft 365 Defender à l’adresse , go <https://security.microsoft.com/> to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **Coffre Links** in the **Policies** section.

     Pour aller directement à la page **Coffre liens,** utilisez <https://security.microsoft.com/safelinksv2> .

  2. Dans la page **Coffre liens,** sélectionnez la stratégie en cliquant sur le nom de la stratégie.
  3. Dans le volant de détails qui s’affiche, faites l’une des étapes suivantes :
     - Pour ajouter une nouvelle stratégie, **sélectionnez + Créer.** Un Assistant se lance pour vous aider à définir vos paramètres de stratégie.
     - Pour modifier une stratégie existante, sélectionnez-la en cliquant sur le nom de la stratégie. Dans le volet d’informations qui s’affiche, sélectionnez **Modifier** dans la section **Paramètres de** protection.
  4. Dans la page **Paramètres de protection,** configurez les paramètres suivants :
     - Activer sélectionner **l’action pour les URL potentiellement malveillantes inconnues dans les messages.**
     - Sélectionnez **Appliquer des liens sûrs aux messages envoyés au sein de l’organisation.**

  Pour plus d’informations, voir [Configurer Coffre de liens dans Microsoft Defender pour Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
