---
title: Notification AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897722"
---
# <a name="notification-aad-connect"></a>Notification AAD Connect

- Assurez-vous que vous êtes autorisé à effectuer l’opération. Les administrateurs globaux y ont accès par défaut. En outre, vous pouvez utiliser le contrôle [d’accès](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) basé sur un rôle pour déléguer l’autorisation d’inscription au collaborateur.
- Assurez-vous que les points de terminaison requis sont activés et non bloqués en raison du pare-feu. Pour plus d’informations, voir [les conditions requises.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- L’inscription peut échouer en raison de la communication sortante soumise à l’inspection SSL par la couche réseau.
- Assurez-vous que vous avez vérifié les paramètres de notification pour Azure AD Connect Health et examinez votre paramètre. Pour comprendre comment configurer les paramètres de notification pour les notifications Azure AD Connect Health, consultez ce [guide.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Pour en savoir plus sur le rapport de synchronisation aAD Connect Health et sur la façon de le télécharger, consultez le rapport de synchronisation au niveau [de l’objet.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Pour résoudre les problèmes d’alertes d’état AAD Connect, suivez le guide de dépannage pour les alertes d’actualité des données d’état AAD Connect et pour les questions fréquemment [posées,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) consultez les questions courantes sur l’installation d’AAD [Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
