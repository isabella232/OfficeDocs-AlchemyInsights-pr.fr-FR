---
title: Configurer les paramètres de confidentialité dans Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090302"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Configurer les paramètres de confidentialité dans Microsoft Edge

Par défaut, si Microsoft Edge est déployé sur des plateformes non Windows, les données de diagnostic et les informations de site ne sont pas envoyées à Microsoft. Toutefois, si Microsoft Edge est déployé sur Windows 10, les données de diagnostic et les informations de site sont envoyées conformément aux paramètres de données de diagnostic Windows [utilisateurs.](https://go.microsoft.com/fwlink/?linkid=2132472)

Pour configurer la façon dont Microsoft Edge collecte de données pour votre organisation, utilisez les stratégies de groupe suivantes :
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) permet de signaler les données relatives à l’utilisation et aux incidents.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) envoie des informations de site utilisées pour améliorer services Microsoft.

Pour plus d’informations, voir [Configurer les paramètres de stratégie.](https://go.microsoft.com/fwlink/?linkid=2132577)
