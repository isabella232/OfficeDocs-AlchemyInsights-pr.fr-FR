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
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="e0e2c-102">AIP : les stratégies ne s’exécutent pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="e0e2c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="e0e2c-103">Azure information protection : les stratégies ne s’exécutent pas comme prévu, consultez les instructions suivantes pour obtenir des informations sur plusieurs problèmes de stratégie :</span><span class="sxs-lookup"><span data-stu-id="e0e2c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="e0e2c-104">Si vous rencontrez des problèmes avec les marques visuelles, passez en revue l’article [Lorsque les marques visuelles sont appliquées](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="e0e2c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="e0e2c-105">Si vous rencontrez des problèmes avec l’étiquetage automatique, passez en revue [Configuration des conditions de classification automatique et recommandée pour Azure information protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) et [Éléments recherchés par les types d’informations sensibles](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="e0e2c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="e0e2c-106">Si vous rencontrez des problèmes avec la protection Native/pfile, veuillez consulter [Configuration de l’API de fichier](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="e0e2c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="e0e2c-107">Vérifiez si vous utilisez des stratégies d’étendue qui ne sont pas configurées correctement : [Configuration de la stratégie Azure information protection pour des utilisateurs spécifiques à l’aide de stratégies étendues](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="e0e2c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="e0e2c-108">Si l’étiquetage automatique ne fonctionne pas pour Outlook lorsque vous joignez un document étiqueté, vérifiez que DRMEncryptProperty n’est pas défini comme décrit ici : [Paramètres de Registre IRM pour la sécurité](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="e0e2c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="e0e2c-109">Si vous rencontrez encore des problèmes, collectez les journaux du client Azure information protection et joignez les journaux exportés à ce ticket.</span><span class="sxs-lookup"><span data-stu-id="e0e2c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="e0e2c-110">Ouvrez un document Office ou créez un courrier électronique dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="e0e2c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="e0e2c-111">Cliquez sur **Protection/confidentialité** > **Aide et commentaires**.</span><span class="sxs-lookup"><span data-stu-id="e0e2c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="e0e2c-112">Cliquez sur **Exporter des journaux**.</span><span class="sxs-lookup"><span data-stu-id="e0e2c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="e0e2c-113">Enregistrez les journaux à l’emplacement de votre choix et joignez-les à cette demande de service.</span><span class="sxs-lookup"><span data-stu-id="e0e2c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="e0e2c-114">Ressources supplémentaires :</span><span class="sxs-lookup"><span data-stu-id="e0e2c-114">Additional resources:</span></span>

- [<span data-ttu-id="e0e2c-115">Configuration d’une étiquette pour les marques visuelles pour Azure information protection</span><span class="sxs-lookup"><span data-stu-id="e0e2c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="e0e2c-116">Consultez la documentation sur Azure information protection</span><span class="sxs-lookup"><span data-stu-id="e0e2c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e0e2c-117">Utiliser des étiquettes de confidentialité dans les applications Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e0e2c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

