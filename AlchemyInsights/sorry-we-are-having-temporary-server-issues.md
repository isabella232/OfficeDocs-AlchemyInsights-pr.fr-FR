---
title: Résolution des problèmes d'applications Microsoft 365 Désolé... Nous avons un message de problèmes de serveur temporaires
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835269"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="6d949-102">Résolution du message des applications Microsoft 365 « Désolé, nous avons des problèmes de serveur temporaires »</span><span class="sxs-lookup"><span data-stu-id="6d949-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="6d949-103">Si vous recevez ce message, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="6d949-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6d949-104">Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour confirmer qu'ils ne bloquent pas l'accès Internet aux applications Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d949-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="6d949-105">Voir [URL et plages d'adresses IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="6d949-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6d949-106">Go to **Start**  >  **Run**, and then type **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="6d949-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6d949-107">Assurez-vous que les services suivants sont tous en cours d'exécution :</span><span class="sxs-lookup"><span data-stu-id="6d949-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6d949-108">Configuration automatique des appareils connectés au réseau</span><span class="sxs-lookup"><span data-stu-id="6d949-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6d949-109">Service de liste réseau</span><span class="sxs-lookup"><span data-stu-id="6d949-109">Network List Service</span></span>
    - <span data-ttu-id="6d949-110">Sensibilisation de l'emplacement réseau</span><span class="sxs-lookup"><span data-stu-id="6d949-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6d949-111">Windows Journal des événements</span><span class="sxs-lookup"><span data-stu-id="6d949-111">Windows Event Log</span></span>

<span data-ttu-id="6d949-112">Si l'un de ces services n'est pas en cours d'exécution, essayez de le démarrer.</span><span class="sxs-lookup"><span data-stu-id="6d949-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6d949-113">Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :</span><span class="sxs-lookup"><span data-stu-id="6d949-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6d949-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="6d949-114">**sfc /scannow**</span></span>

<span data-ttu-id="6d949-115">Une fois cette commande terminé, redémarrez l'ordinateur.</span><span class="sxs-lookup"><span data-stu-id="6d949-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6d949-116">Pour plus d'informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » erreur lors de l'activation.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="6d949-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>