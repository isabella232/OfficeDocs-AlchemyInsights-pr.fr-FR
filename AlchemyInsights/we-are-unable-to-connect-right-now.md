---
title: "Problème d'activation : nous ne pouvons pas nous connecter pour le moment"
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806440"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="3599e-102">Résolution du message des applications Microsoft 365 « Nous ne pouvons pas nous connecter pour le moment »</span><span class="sxs-lookup"><span data-stu-id="3599e-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="3599e-103">Si vous recevez ce message, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="3599e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3599e-104">Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour confirmer qu'ils ne bloquent pas l'accès Internet aux applications Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3599e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3599e-105">Voir [URL et plages d'adresses IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="3599e-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="3599e-106">Go to **Start**  >  **Run**, and then type **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="3599e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="3599e-107">Assurez-vous que les services suivants sont tous en cours d'exécution :</span><span class="sxs-lookup"><span data-stu-id="3599e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="3599e-108">Configuration automatique des appareils connectés au réseau</span><span class="sxs-lookup"><span data-stu-id="3599e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="3599e-109">Service de liste réseau</span><span class="sxs-lookup"><span data-stu-id="3599e-109">Network List Service</span></span>
    - <span data-ttu-id="3599e-110">Sensibilisation de l'emplacement réseau</span><span class="sxs-lookup"><span data-stu-id="3599e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="3599e-111">Windows Journal des événements</span><span class="sxs-lookup"><span data-stu-id="3599e-111">Windows Event Log</span></span>

<span data-ttu-id="3599e-112">Si l'un de ces services n'est pas en cours d'exécution, essayez de le démarrer.</span><span class="sxs-lookup"><span data-stu-id="3599e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="3599e-113">Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :</span><span class="sxs-lookup"><span data-stu-id="3599e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="3599e-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="3599e-114">**sfc /scannow**</span></span>

<span data-ttu-id="3599e-115">Une fois cette commande terminé, redémarrez l'ordinateur.</span><span class="sxs-lookup"><span data-stu-id="3599e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="3599e-116">Pour plus d'informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » lorsque vous activez Office à partir de Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="3599e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>