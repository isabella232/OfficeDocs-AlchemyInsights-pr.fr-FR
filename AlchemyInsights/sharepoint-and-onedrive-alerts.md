---
title: Retarde la réception des alertes OneDrive et SharePoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563508"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="7f2a6-102">Retarde la réception des alertes OneDrive et SharePoint</span><span class="sxs-lookup"><span data-stu-id="7f2a6-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="7f2a6-103">Vérifiez d’abord le dossier courrier indésirable dans votre courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="7f2a6-104">Si **toutes les alertes provenant de plusieurs fichiers ou bibliothèques sont retardées**, visitez le [tableau de bord État du service](https://portal.office.com/adminportal/home?ref=/servicehealth) pour vérifier les avis/incidents susceptibles de se produire avec SharePoint ou Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="7f2a6-105">Le problème peut être lié à la capacité d’alerte ou aux retards d’alertes de SharePoint par le biais d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="7f2a6-106">Notez également si d’autres e-mails sont remis (si ce n’est pas le cas), le problème est probablement lié à Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="7f2a6-107">Si **une alerte individuelle d’un fichier ou d’une bibliothèque spécifique n’est pas remise**, essayez de la supprimer et de la recréer.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="7f2a6-108">Consultez la rubrique [Manage, View, or delete SharePoint Alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pour recréer l’alerte.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="7f2a6-109">Les alertes ne peuvent pas être envoyées à un groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="7f2a6-110">Seuls les groupes Security et O365 sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="7f2a6-111">Vous ne pouvez pas personnaliser les modèles de courrier électronique d’alerte.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="7f2a6-112">Vous devez utiliser le flux de travail Microsoft Flow ou SharePoint Designer pour y parvenir.</span><span class="sxs-lookup"><span data-stu-id="7f2a6-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
