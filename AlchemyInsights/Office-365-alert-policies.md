---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312685"
---
# <a name="alert-policies"></a>Stratégies d’alerte

Microsoft 365 contient des [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) stratégies d’alerte par défaut qui déclenchent des alertes pour les organisations ayant un abonnement Microsoft 365 Entreprise ou Microsoft 365 pour le gouvernement américain E1/G1, E3/G3 ou E5/G5. Par conséquent, les administrateurs peuvent recevoir une notification par courrier électronique d’alerte envoyée par Office365Alerts@microsoft.com avec une ligne d’objet telle que « Une alerte de faible gravité : nom de stratégie d’alerte ». Les notifications d’alerte sont envoyées lorsque des alertes sont déclenchées pour des activités courantes, par exemple lorsque les utilisateurs :

- Créez des règles de boîte de réception qui envoient le courrier électronique.
- Attribuez des autorisations à leur boîte aux lettres.
- Partagez ou supprimez un grand nombre de fichiers dans SharePoint partage de fichiers.
- Créer des recherches eDiscovery et exporter des résultats de recherche.

Pour examiner et agir sur une alerte :

1. Effectuez l’une des étapes suivantes :
   - In the Centre de conformité Microsoft 365 at <https://compliance.microsoft.com> , go to **Alerts**. Ou, pour aller directement à la page **Alertes,** utilisez <https://compliance.microsoft.com/compliancealerts> .
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Incidents &** \> **alerts**. Ou, pour aller directement à la page **Alertes,** utilisez <https://security.microsoft.com/alerts> .
2. Cliquez sur une alerte pour afficher une page volante avec des informations sur l’alerte.

Vous pouvez prendre des mesures sur une alerte, telle que la [suppression d’une règle de boîte de réception suspecte.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Sinon, vous pouvez simplement fermer l’alerte en cliquant sur **Résoudre** dans la page volante d’alerte.

Pour plus d’informations sur la configuration et la gestion des stratégies d’alerte, consultez [cet article.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Important**: les notifications par courrier électronique d’alerte de Microsoft ne vous demanderont jamais de faire les choses suivantes :

- Fournir un mot de passe
- Vérifier les détails de sécurité de votre compte
- Se ré-authentifier

Si vous recevez un message électronique avec ces types de demandes, il n’a pas été envoyé par Microsoft et doit être considéré comme une tentative de hameçonnage. Si vous recevez un message avec ces types de demandes, [signalez-le à Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)
