---
title: L’inventaire logiciel est manquant ou incorrect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658050"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="75615-102">L’inventaire logiciel est manquant ou incorrect</span><span class="sxs-lookup"><span data-stu-id="75615-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="75615-103">L'inventaire des logiciels dans le cadre de la gestion des menaces et des vulnérabilités (GVT) est une liste des logiciels connus dans votre organisation avec les énumérations officielles de la plateforme commune (CPE).</span><span class="sxs-lookup"><span data-stu-id="75615-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="75615-104">Les produits logiciels sans CPE officielles n'ont pas de vulnérabilités publiées.</span><span class="sxs-lookup"><span data-stu-id="75615-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="75615-105">L'inventaire comprend également des informations telles que le nom du fournisseur, le nombre de faiblesses, les menaces et le nombre d'appareils exposés.</span><span class="sxs-lookup"><span data-stu-id="75615-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="75615-106">Les modifications apportées aux logiciels sur les appareils sont généralement reflétées dans les portails de sécurité en moins de deux heures.</span><span class="sxs-lookup"><span data-stu-id="75615-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="75615-107">Toutefois, cela peut parfois prendre plus de temps.</span><span class="sxs-lookup"><span data-stu-id="75615-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="75615-108">Il est actuellement impossible de forcer une synchronisation ; il s'agit d'une évaluation continue.</span><span class="sxs-lookup"><span data-stu-id="75615-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="75615-109">Si vous avez apporté un changement de logiciel et que la modification n’est pas reflétée avec précision dans TVM après 5 heures, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="75615-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="75615-110">Consultez la section sur les preuves du logiciel pour comprendre comment le logiciel a été détecté.</span><span class="sxs-lookup"><span data-stu-id="75615-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="75615-111">Assurez-vous que le logiciel est pris en charge.</span><span class="sxs-lookup"><span data-stu-id="75615-111">Make sure that the software is supported.</span></span> <span data-ttu-id="75615-112">Le logiciel peut être visible uniquement au niveau de l’appareil, même s’il n’est actuellement pas pris en charge par la gestion des menaces et vulnérabilités.</span><span class="sxs-lookup"><span data-stu-id="75615-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="75615-113">Toutefois, seules des données limitées sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="75615-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="75615-114">Pour savoir comment signaler l’erreur d’accès à partir du portail, consultez [Signaler une inexactitude](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="75615-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="75615-115">**Remarque** : signaler une inexactitude à partir du portail MDE est un canal à sens unique vers l'ingénierie.</span><span class="sxs-lookup"><span data-stu-id="75615-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="75615-116">Si le problème est urgent, ouvrez un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="75615-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="75615-117">Pour plus d’informations, voir [Inventaire logiciel – gestion des menaces et des vulnérabilités](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="75615-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>