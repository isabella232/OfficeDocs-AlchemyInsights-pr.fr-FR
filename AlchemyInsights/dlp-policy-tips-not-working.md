---
title: Les conseils de stratégie DLP ne fonctionnent pas
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932584"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="c9b5c-102">Problèmes de Conseil de stratégie DLP</span><span class="sxs-lookup"><span data-stu-id="c9b5c-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="c9b5c-103">**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c9b5c-104">Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c9b5c-105">Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c9b5c-106">Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c9b5c-107">Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c9b5c-108">Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c9b5c-109">**Conseils de stratégie DLP**</span><span class="sxs-lookup"><span data-stu-id="c9b5c-109">**DLP policy tips**</span></span>

<span data-ttu-id="c9b5c-110">Lorsque vous utilisez des **stratégies DLP**, les utilisateurs peuvent être avertis d’une violation de stratégie à l’aide de **conseils de stratégie**.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="c9b5c-111">Les administrateurs peuvent configurer des conseils de stratégie à afficher pendant le test de leur stratégie DLP ou lorsque la stratégie est en mode d’application complète.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="c9b5c-112">Pour configurer des conseils de stratégie sur votre stratégie DLP dans le centre de sécurité et de conformité en mode d’application complète, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="c9b5c-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="c9b5c-113">Assurez-vous que les conseils de stratégie ont été **activés** sur la règle DLP en suivant les étapes [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="c9b5c-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="c9b5c-114">Vérifiez que votre **contenu correspond** à ce qui est **requis** pour déclencher la règle décrite dans cet article [ici](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c9b5c-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c9b5c-115">Les conseils de stratégie sont affichés dans OWA et Outlook.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="c9b5c-116">Toutefois, lorsque vous utilisez **Outlook 2013 ou une version ultérieure**, les conseils de stratégie s’affichent uniquement dans certaines conditions.</span><span class="sxs-lookup"><span data-stu-id="c9b5c-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="c9b5c-117">Ces conditions sont répertoriées ci-dessous : [conditions prises en charge pour Outlook 2013 ou version ultérieure pour l’affichage des conseils de stratégie](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="c9b5c-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="c9b5c-118">Pour plus d’informations sur les conseils de stratégie DLP, voir : [afficher les conseils de stratégie pour les stratégies DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="c9b5c-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  