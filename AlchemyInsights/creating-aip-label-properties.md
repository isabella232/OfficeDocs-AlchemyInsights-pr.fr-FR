---
title: Création de stratégies d’étiquette AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542099"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="42bb5-102">Création de stratégies d’étiquette AIP</span><span class="sxs-lookup"><span data-stu-id="42bb5-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="42bb5-103">Azure information protection (AIP) les étiquettes peuvent être utilisées avec la plage complète de données qu’une organisation crée et stocke généralement, de la classification de données personnelles la plus faible à la classification la plus élevée des données hautement confidentielles.</span><span class="sxs-lookup"><span data-stu-id="42bb5-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="42bb5-104">Les stratégies Azure information protection s’appliquent au client classique Azure information protection (AIP) et non au [client d’étiquetage unifié AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="42bb5-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="42bb5-105">Vous pouvez configurer plusieurs éléments dans une stratégie AIP, notamment des options telles que :</span><span class="sxs-lookup"><span data-stu-id="42bb5-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="42bb5-106">Option pour laquelle l’étiquette permettra aux administrateurs ou aux utilisateurs de classer et de protéger (facultatif) les documents et les e-mails</span><span class="sxs-lookup"><span data-stu-id="42bb5-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="42bb5-107">Option permettant d’appliquer la classification lorsque les utilisateurs enregistrent et envoient du courrier électronique</span><span class="sxs-lookup"><span data-stu-id="42bb5-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="42bb5-108">Option pour étiqueter automatiquement un message électronique, en fonction de ses pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="42bb5-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="42bb5-109">Option permettant de contrôler si la barre de protection des informations est affichée dans les applications Office</span><span class="sxs-lookup"><span data-stu-id="42bb5-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="42bb5-110">Pour obtenir des options supplémentaires et des informations sur les stratégies Azure information protection, voir : [Overview of the Azure information protection Policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="42bb5-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="42bb5-111">Pour les autres ressources utiles concernant les stratégies AIP, consultez les ressources suivantes :</span><span class="sxs-lookup"><span data-stu-id="42bb5-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="42bb5-112">Didacticiel : configurer les paramètres de stratégie Azure information protection et créer une nouvelle étiquette</span><span class="sxs-lookup"><span data-stu-id="42bb5-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="42bb5-113">Configuration de la stratégie Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="42bb5-114">Créer et configurer des étiquettes de confidentialité ainsi que leurs stratégies</span><span class="sxs-lookup"><span data-stu-id="42bb5-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="42bb5-115">Guides de procédures pour les scénarios courants qui utilisent Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="42bb5-116">Consulter la documentation Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="42bb5-117">Configuration requise pour Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="42bb5-118">Didacticiel de démarrage rapide pour Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="42bb5-119">Télécharger le client Azure information protection</span><span class="sxs-lookup"><span data-stu-id="42bb5-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)