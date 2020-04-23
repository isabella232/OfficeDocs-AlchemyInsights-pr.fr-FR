---
title: Notifications d’alerte SharePoint non remises
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742045"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="aa5c9-102">Notifications d’alerte SharePoint non remises</span><span class="sxs-lookup"><span data-stu-id="aa5c9-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="aa5c9-103">Vérifiez le dossier de courrier indésirable dans votre courrier électronique, car des alertes pourraient y figurer.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="aa5c9-104">Déterminez si **toutes les alertes ne sont pas remises** ou si **une alerte individuelle** d’un fichier ou d’une bibliothèque spécifique n’est pas remise.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="aa5c9-105">**Les alertes individuelles ne sont pas remises**: si une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise, vous pouvez essayer de la supprimer et de la recréer.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="aa5c9-106">Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pour recréer l’alerte.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="aa5c9-107">**Toutes les alertes ne sont pas remises**: si toutes les alertes provenant de plusieurs fichiers ou bibliothèques ne sont pas remises, consultez le [tableau de bord État du service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="aa5c9-108">Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="aa5c9-109">Il est également important de noter si d’autres e-mails sont remis et, si ce n’est pas le cas, le problème est probablement lié à Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="aa5c9-110">FAQ sur les alertes :</span><span class="sxs-lookup"><span data-stu-id="aa5c9-110">FAQ on alerts:</span></span>

- <span data-ttu-id="aa5c9-111">Il n’est pas possible d’envoyer des alertes à un groupe de distribution, seuls les groupes Security et O365 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="aa5c9-112">Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte ; vous devez utiliser le flux de travail Microsoft FLOW ou SharePoint Designer pour y parvenir.</span><span class="sxs-lookup"><span data-stu-id="aa5c9-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="aa5c9-113">Informations supplémentaires :</span><span class="sxs-lookup"><span data-stu-id="aa5c9-113">More Information:</span></span>

- <span data-ttu-id="aa5c9-114">**Configuration**des alertes : pour plus d’informations sur la configuration des alertes, consultez [la rubrique créer une alerte pour être averti lorsqu’un fichier ou un dossier est modifié dans SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="aa5c9-115">**Dépannage des alertes**: pour plus d’informations sur la résolution des alertes, consultez la rubrique [les utilisateurs ne reçoivent pas les notifications d’alerte SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="aa5c9-116">**Stratégies avancées d’alerte de conformité O365**: pour plus d’informations sur la configuration de ces alertes, consultez [la rubrique stratégies d’alerte de conformité](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="aa5c9-117">**Journaux d’audit SharePoint et OneDrive**: pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="aa5c9-118">**Alertes envoyées par protection avancée contre les menaces**: consultez la rubrique [ATP pour SharePoint et OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="aa5c9-119">**Alertes envoyées par les stratégies de protection contre la perte de données**: consultez la rubrique [notifications par courrier électronique pour les stratégies DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="aa5c9-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="aa5c9-120">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="aa5c9-120">Related Topics</span></span>

<span data-ttu-id="aa5c9-121">Vous souhaitez essayer Microsoft Flow dans SharePoint Online ?</span><span class="sxs-lookup"><span data-stu-id="aa5c9-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="aa5c9-122">Créer un flux</span><span class="sxs-lookup"><span data-stu-id="aa5c9-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="aa5c9-123">SharePoint et flux</span><span class="sxs-lookup"><span data-stu-id="aa5c9-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
