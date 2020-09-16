---
title: 'Problème d’activation : nous ne pouvons pas vous connecter pour le moment'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725981"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="4b09b-102">Résolution du message « nous ne parvenons pas à se connecter pour les applications Microsoft 365 »</span><span class="sxs-lookup"><span data-stu-id="4b09b-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="4b09b-103">Si vous recevez ce message, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="4b09b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4b09b-104">Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b09b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4b09b-105">Consultez la rubrique [URL et plages d’adresses IP Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="4b09b-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4b09b-106">Accédez à **Démarrer**l'  >  **exécution**, puis tapez **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="4b09b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4b09b-107">Assurez-vous que les services suivants sont en cours d’exécution :</span><span class="sxs-lookup"><span data-stu-id="4b09b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4b09b-108">Configuration automatique des périphériques connectés au réseau</span><span class="sxs-lookup"><span data-stu-id="4b09b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4b09b-109">Service de liste de réseaux</span><span class="sxs-lookup"><span data-stu-id="4b09b-109">Network List Service</span></span>
    - <span data-ttu-id="4b09b-110">Connaissance des emplacements réseau</span><span class="sxs-lookup"><span data-stu-id="4b09b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4b09b-111">Windows Journal des événements</span><span class="sxs-lookup"><span data-stu-id="4b09b-111">Windows Event Log</span></span>

<span data-ttu-id="4b09b-112">Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer.</span><span class="sxs-lookup"><span data-stu-id="4b09b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4b09b-113">Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :</span><span class="sxs-lookup"><span data-stu-id="4b09b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4b09b-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="4b09b-114">**sfc /scannow**</span></span>

<span data-ttu-id="4b09b-115">Une fois que cette commande est terminée, redémarrez l’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="4b09b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4b09b-116">Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Veuillez réessayer plus tard» lorsque vous activez Office à partir de Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="4b09b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>