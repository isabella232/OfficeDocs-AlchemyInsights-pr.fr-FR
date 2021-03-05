---
title: Problème avec AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453292"
---
# <a name="problem-with-aad-connect-health"></a>Problème avec AAD Connect Health

- Assurez-vous que vous êtes autorisé à effectuer l’opération. Les administrateurs globaux y ont accès par défaut. En outre, vous pouvez utiliser le contrôle [d’accès](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) basé sur un rôle pour déléguer l’autorisation d’inscription au collaborateur.
- Assurez-vous que les points de terminaison requis sont activés et non bloqués en raison du pare-feu. Pour plus d’informations, voir [les conditions requises.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- L’inscription peut échouer en raison de la communication sortante soumise à l’inspection SSL par la couche réseau.
- Assurez-vous que vous avez vérifié les paramètres de notification pour Azure AD Connect Health. Veuillez consulter votre paramètre. Ce [guide peut](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vous aider à comprendre comment configurer les paramètres de notification pour les notifications d’état d’état Azure AD Connect.
- Pour en savoir plus sur le rapport de synchronisation aAD Connect Health et sur la façon de le télécharger, consultez le rapport de synchronisation au niveau [de l’objet.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Pour résoudre les problèmes d’alertes d’état AAD Connect, suivez le guide de dépannage pour les alertes d’actualité des données d’état [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) et pour les questions fréquemment posées, consultez les questions courantes sur l’installation [d’AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
