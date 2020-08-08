---
title: Supprimer un canal privé Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431445"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="aef69-102">Supprimer un canal privé Teams</span><span class="sxs-lookup"><span data-stu-id="aef69-102">Delete a Teams private channel</span></span>

<span data-ttu-id="aef69-103">Microsoft a connaissance d’un problème lors de la suppression d’un canal privé Teams si les stratégies de rétention SharePoint sont activées pour le site SharePoint sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="aef69-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="aef69-104">Microsoft travaille à l’élaboration d’un correctif.</span><span class="sxs-lookup"><span data-stu-id="aef69-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="aef69-105">En attendant, vous pouvez utiliser les solutions de contournement suivantes pour supprimer le canal privé.</span><span class="sxs-lookup"><span data-stu-id="aef69-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="aef69-106">**Exclure l’équipe ou la collection de sites de la stratégie de rétention SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="aef69-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="aef69-107">Accédez au Portail d’administration Office 365 et sélectionnez **Afficher toutes** dans le volet de navigation gauche.</span><span class="sxs-lookup"><span data-stu-id="aef69-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="aef69-108">Sous **Centres d’administration**, accédez à **Sécurité et conformité** > **Protection contre la perte de données** > **stratégie**.</span><span class="sxs-lookup"><span data-stu-id="aef69-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="aef69-109">Identifiez les stratégies qui s’appliquent aux sites SharePoint et modifiez la stratégie de sorte que le site SharePoint pour l’équipe contenant le canal privé ne soit pas inclus dans la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="aef69-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="aef69-110">Enregistrez la stratégie.</span><span class="sxs-lookup"><span data-stu-id="aef69-110">Save the policy.</span></span>
    <span data-ttu-id="aef69-111">La prise en compte des paramètres de stratégie peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="aef69-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="aef69-112">Une fois le site exclu, vous pouvez supprimer le canal privé.</span><span class="sxs-lookup"><span data-stu-id="aef69-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="aef69-113">Vous ***pouvez*** être en mesure de supprimer le canal privé à l’aide de Microsoft Teams sur votre appareil Android.</span><span class="sxs-lookup"><span data-stu-id="aef69-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="aef69-114">Pour plus d’informations sur SharePoint, consultez [Impossible de supprimer des éléments dans SharePoint Online ou OneDrive Entreprise](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="aef69-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>