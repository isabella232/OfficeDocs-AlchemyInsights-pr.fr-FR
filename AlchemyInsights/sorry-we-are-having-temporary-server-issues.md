---
title: Résolution des applications Microsoft 365 Désolé, un message de problèmes de serveur temporaire s’affiche.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582701"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="58e3d-102">Résolution des applications Microsoft 365 les applications « Désolé, nous rencontrons des problèmes de serveur temporaires »</span><span class="sxs-lookup"><span data-stu-id="58e3d-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="58e3d-103">Si vous recevez ce message, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="58e3d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="58e3d-104">Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="58e3d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="58e3d-105">Voir [URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="58e3d-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="58e3d-106">Accédez à **Démarrer**l'  >  **exécution**, puis tapez **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="58e3d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="58e3d-107">Assurez-vous que les services suivants sont en cours d’exécution :</span><span class="sxs-lookup"><span data-stu-id="58e3d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="58e3d-108">Configuration automatique des périphériques connectés au réseau</span><span class="sxs-lookup"><span data-stu-id="58e3d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="58e3d-109">Service de liste de réseaux</span><span class="sxs-lookup"><span data-stu-id="58e3d-109">Network List Service</span></span>
    - <span data-ttu-id="58e3d-110">Connaissance des emplacements réseau</span><span class="sxs-lookup"><span data-stu-id="58e3d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="58e3d-111">Windows Journal des événements</span><span class="sxs-lookup"><span data-stu-id="58e3d-111">Windows Event Log</span></span>

<span data-ttu-id="58e3d-112">Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer.</span><span class="sxs-lookup"><span data-stu-id="58e3d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="58e3d-113">Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :</span><span class="sxs-lookup"><span data-stu-id="58e3d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="58e3d-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="58e3d-114">**sfc /scannow**</span></span>

<span data-ttu-id="58e3d-115">Une fois que cette commande est terminée, redémarrez l’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="58e3d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="58e3d-116">Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Réessayez ultérieurement» lorsque vous procédez à l’activation](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="58e3d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>