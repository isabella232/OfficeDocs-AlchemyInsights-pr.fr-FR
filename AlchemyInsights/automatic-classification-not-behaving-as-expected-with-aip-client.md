---
title: Classification automatique non conforme au client AIP
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820896"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Classification automatique non conforme au client AIP

La classification automatique ne s’utilise pas comme prévu, suivez les recommandations suivantes :

1. Si vous rencontrez des problèmes avec l’étiquetage automatique, consultez [Configuration des conditions de classification automatique et recommandée pour Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) et [Éléments recherchés par les types d’informations sensibles](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Vérifiez si vous utilisez des stratégies d’étendue qui ne sont pas configurées correctement : [Configuration de la stratégie Azure information protection pour des utilisateurs spécifiques à l’aide de stratégies étendues](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Si l’étiquetage automatique ne fonctionne pas pour Outlook lorsque vous joignez un document étiqueté, vérifiez que `DRMEncryptProperty` n’est pas défini comme décrit ici : [Paramètres de Registre IRM pour la sécurité](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Si vous avez utilisé les [types d’informations intégrés](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) pour votre stratégie Azure information protection, vérifiez que votre contenu correspond au format attendu.
5. Vérifiez que l’étiquette est correctement configurée pour **Automatique** ou **Recommandée**. (L’étiquetage **automatique** est disponible pour toutes les applications Microsoft 365, tandis que **Recommandé** est disponible pour toutes les applications Microsoft 365 à l’exception d’Outlook.)
6. Vous ne pouvez pas utiliser la classification automatique pour les documents et les messages électroniques qui ont été précédemment étiquetés manuellement ou automatiquement avec une classification supérieure.  Pour plus d’information, consultez : [Comment les étiquettes automatiques ou recommandées sont appliquées](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Si vous rencontrez encore des problèmes, collectez les journaux du client Azure information protection et joignez les journaux exportés aux tickets de support. Pour exporter des journaux Azure information protection :
    - Ouvrez un document Office ou créez un courrier électronique dans Outlook.
    - Cliquez sur **Protection/confidentialité** > **Aide et commentaires**.
    - Cliquez sur **Exporter des journaux**.
    - Enregistrez les journaux à l’emplacement de votre choix et joignez-les à votre demande de service.

Pour plus d’informations, voir :

- [Comment configurer les conditions de classification automatique et recommandée pour Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guides de procédures pour les scénarios courants utilisant Azure information protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Consultez la documentation sur Azure information protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Examiner les abonnements et fonctionnalités d’Azure information protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Configuration requise pour Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Didacticiel de démarrage rapide pour Azure information protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Télécharger l’application Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
