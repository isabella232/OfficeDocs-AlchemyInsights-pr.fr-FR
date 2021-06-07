---
title: Expédition de disque dans le service d’importation Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721691"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="c8e1f-102">Expédition de disque dans le service d’importation Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c8e1f-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="c8e1f-103">Utilisez l’expédition de disque en copiant les fichiers PST sur un disque dur, puis en expédiant le disque dur à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="c8e1f-104">Pour démarrer la tâche :</span><span class="sxs-lookup"><span data-stu-id="c8e1f-104">To start the job:</span></span>

1. <span data-ttu-id="c8e1f-105">Dans le Centre de conformité Microsoft 365 sous **Gouvernance des informations**, sélectionnez **Importer**.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="c8e1f-106">Sélectionnez **Choisir le type de tâche d’importation**, puis sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="c8e1f-107">Pour afficher les étapes de cette option d’importation, sélectionnez **Expédier des disques durs à l’un de nos emplacements physiques**.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="c8e1f-108">Voici quelques éléments à retenir :</span><span class="sxs-lookup"><span data-stu-id="c8e1f-108">Here are some things to remember:</span></span>

- <span data-ttu-id="c8e1f-109">Le rôle Importation/Exportation de boîtes aux lettres doit vous avoir été attribué dans Exchange Online pour pouvoir importer des fichiers PST dans des boîtes aux lettres Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="c8e1f-110">Les performances peuvent être affectées pour les fichiers PST supérieurs à 20 Go.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="c8e1f-111">Seuls les lecteurs SSD 2,5 ou 2,5 pouces ou les disques durs internes 3,5 pouces SATA II/III sont pris en charge.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="c8e1f-112">Le disque dur contenant des fichiers PST doit être chiffré avec BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="c8e1f-113">Le tarif pour importer des fichiers PST dans les boîtes aux lettres Microsoft 365 via l’expédition de disque s’élève à 2 $ USD par Go de données.</span><span class="sxs-lookup"><span data-stu-id="c8e1f-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="c8e1f-114">Pour plus d’informations sur l’utilisation de la méthode d’expédition de lecteur pour importer des fichiers PST, consultez [Utiliser l’expédition de lecteur pour importer les fichiers PST de votre organisation](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="c8e1f-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>