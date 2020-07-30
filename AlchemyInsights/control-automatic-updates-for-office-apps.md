---
title: Contrôler les mises à jour automatiques pour les applications Office
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
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431446"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="16a48-102">Contrôler les mises à jour automatiques pour les applications Office</span><span class="sxs-lookup"><span data-stu-id="16a48-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="16a48-103">Par défaut, les mises à jour des applications Office sont téléchargées automatiquement et appliquées en arrière-plan, sans aucune intervention de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="16a48-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="16a48-104">Toutefois, les administrateurs peuvent contrôler la manière dont les mises à jour sont appliquées à l’aide des paramètres de mise à jour d’Office.</span><span class="sxs-lookup"><span data-stu-id="16a48-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="16a48-105">Les paramètres de mise à jour permettent aux administrateurs d’activer ou de désactiver les mises à jour automatiques, d’afficher ou de masquer le bouton **Mettre à jour maintenant** dans Office, définir des échéances de mise à jour, etc.</span><span class="sxs-lookup"><span data-stu-id="16a48-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="16a48-106">Pour plus d'informations, consultez :</span><span class="sxs-lookup"><span data-stu-id="16a48-106">For detailed information, see:</span></span>

- [<span data-ttu-id="16a48-107">Définir les paramètres de mise à jour pour Office</span><span class="sxs-lookup"><span data-stu-id="16a48-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="16a48-108">Les mises à jour automatiques pour Office ne sont pas activées</span><span class="sxs-lookup"><span data-stu-id="16a48-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="16a48-109">Définir la façon dont Office est mis à jour après l’installation</span><span class="sxs-lookup"><span data-stu-id="16a48-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="16a48-110">Pour passer en revue les paramètres de mises à jour existants appliqués à un ordinateur client, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="16a48-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="16a48-111">Ouvrez l’Éditeur du registre en accédant à **Démarrer** > **Exécuter** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="16a48-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="16a48-112">Accédez à l’emplacement suivant et passez en revue les paramètres de mise à jour d’Office :</span><span class="sxs-lookup"><span data-stu-id="16a48-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="16a48-113">a.</span><span class="sxs-lookup"><span data-stu-id="16a48-113">a.</span></span> <span data-ttu-id="16a48-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="16a48-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="16a48-115">b.</span><span class="sxs-lookup"><span data-stu-id="16a48-115">b.</span></span> <span data-ttu-id="16a48-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="16a48-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="16a48-117">**Remarque**  si la clé OfficeMgmtCOM est activée, vous pouvez afficher le message « Les mises à jour sont gérées par votre administrateur système » dans **Office** > **Compte** > **Mises à jour d’Office**.</span><span class="sxs-lookup"><span data-stu-id="16a48-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="16a48-118">Pour plus d’informations, consultez [Gestion des mises à jour vers Microsoft 365 Apps avec Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="16a48-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  