---
title: Créer et gérer des balises ou des groupes d’appareils
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
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721697"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="a86f3-102">Créer et gérer des balises ou des groupes d’appareils</span><span class="sxs-lookup"><span data-stu-id="a86f3-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="a86f3-103">Ajoutez des balises sur les appareils pour créer une affiliation de groupe logique.</span><span class="sxs-lookup"><span data-stu-id="a86f3-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="a86f3-104">Les balises d’appareil prennent en charge le mappage approprié du réseau, ce qui vous permet d’attacher différentes balises pour capturer le contexte et d’activer la création de liste dynamique dans le cadre d’un incident.</span><span class="sxs-lookup"><span data-stu-id="a86f3-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="a86f3-105">Les balises peuvent être utilisées comme filtre dans l’affichage Liste des appareils ou pour regrouper des appareils.</span><span class="sxs-lookup"><span data-stu-id="a86f3-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="a86f3-106">Pour plus d’informations sur le regroupement d’appareils, consultez [Créer et gérer des balises d’appareil](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="a86f3-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="a86f3-107">Vous pouvez ajouter des balises sur les appareils en :</span><span class="sxs-lookup"><span data-stu-id="a86f3-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="a86f3-108">Utilisation du portail</span><span class="sxs-lookup"><span data-stu-id="a86f3-108">Using the portal</span></span>

- <span data-ttu-id="a86f3-109">Définition d’une valeur de clé de Registre</span><span class="sxs-lookup"><span data-stu-id="a86f3-109">Setting a registry key value</span></span>
 
<span data-ttu-id="a86f3-110">**Remarque :** Il peut y avoir une latence entre le moment où une balise est ajoutée à un appareil et sa disponibilité dans la liste des appareils et la page de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="a86f3-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="a86f3-111">Pour ajouter des balises d’appareil à l’aide de l’API, consultez [Ajouter ou supprimer des balises d’appareil API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="a86f3-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="a86f3-112">Ajouter et gérer des balises d’appareil à l’aide du portail</span><span class="sxs-lookup"><span data-stu-id="a86f3-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="a86f3-113">Sélectionnez l’appareil sur lequel vous souhaitez gérer les balises.</span><span class="sxs-lookup"><span data-stu-id="a86f3-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="a86f3-114">Vous pouvez sélectionner ou rechercher un appareil à partir de l’une des vues suivantes :</span><span class="sxs-lookup"><span data-stu-id="a86f3-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="a86f3-115">**Tableau de bord des opérations de sécurité** Sélectionnez le nom de l’appareil dans la section Principaux appareils associés à des alertes actives.</span><span class="sxs-lookup"><span data-stu-id="a86f3-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="a86f3-116">**File d’attente des alertes** : sélectionnez le nom de l’appareil en regard de l’icône de l’appareil dans la file d’attente des alertes.</span><span class="sxs-lookup"><span data-stu-id="a86f3-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="a86f3-117">**Liste des appareils** : sélectionnez le nom de l’appareil dans la liste des appareils.</span><span class="sxs-lookup"><span data-stu-id="a86f3-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="a86f3-118">**Zone de recherche** : sélectionnez Appareil dans le menu déroulant et entrez le nom de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="a86f3-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="a86f3-119">Vous pouvez également accéder à la page d’alerte via les Affichages de fichier et d’adresse IP.</span><span class="sxs-lookup"><span data-stu-id="a86f3-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="a86f3-120">Sélectionnez **Gérer les balises** dans la ligne des actions de réponse.</span><span class="sxs-lookup"><span data-stu-id="a86f3-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="a86f3-121">Taper pour rechercher ou créer des balises.</span><span class="sxs-lookup"><span data-stu-id="a86f3-121">Type to find or create tags.</span></span>

<span data-ttu-id="a86f3-122">Les balises sont ajoutées à la vue appareil et sont répercutées dans l’affichage Liste des appareils.</span><span class="sxs-lookup"><span data-stu-id="a86f3-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="a86f3-123">Vous pouvez ensuite utiliser le filtre Balises pour afficher la liste des appareils appropriés.</span><span class="sxs-lookup"><span data-stu-id="a86f3-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="a86f3-124">Pour plus d'informations, consultez la rubrique [Créer et gérer des balises d’appareil](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="a86f3-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>