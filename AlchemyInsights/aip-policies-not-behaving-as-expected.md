---
title: 'AIP : les stratégies ne s’exécutent pas comme prévu'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821625"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP : les stratégies ne s’exécutent pas comme prévu

Azure information protection : les stratégies ne s’exécutent pas comme prévu, consultez les instructions suivantes pour obtenir des informations sur plusieurs problèmes de stratégie :

1. Si vous rencontrez des problèmes avec les marques visuelles, passez en revue l’article [Lorsque les marques visuelles sont appliquées](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Si vous rencontrez des problèmes avec l’étiquetage automatique, passez en revue [Configuration des conditions de classification automatique et recommandée pour Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) et [Éléments recherchés par les types d’informations sensibles](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Si vous rencontrez des problèmes avec la protection Native/pfile, veuillez consulter [Configuration de l’API de fichier](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Vérifiez si vous utilisez des stratégies d’étendue qui ne sont pas configurées correctement : [Configuration de la stratégie Azure information protection pour des utilisateurs spécifiques à l’aide de stratégies étendues](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Si l’étiquetage automatique ne fonctionne pas pour Outlook lorsque vous joignez un document étiqueté, vérifiez que DRMEncryptProperty n’est pas défini comme décrit ici : [Paramètres de Registre IRM pour la sécurité](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Si vous rencontrez encore des problèmes, collectez les journaux du client Azure information protection et joignez les journaux exportés à ce ticket.

1. Ouvrez un document Office ou créez un courrier électronique dans Outlook.
2. Cliquez sur **Protection/confidentialité** > **Aide et commentaires**.
3. Cliquez sur **Exporter des journaux**.
4. Enregistrez les journaux à l’emplacement de votre choix et joignez-les à cette demande de service.

Ressources supplémentaires :

- [Configuration d’une étiquette pour les marques visuelles pour Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Consultez la documentation sur Azure information protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utiliser des étiquettes de confidentialité dans les applications Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

