---
title: 'Problème d’activation : nous ne pouvons pas vous connecter pour le moment'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716170"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ac539-102">Correction des applications Office « nous ne parvenons pas à se connecter maintenant »</span><span class="sxs-lookup"><span data-stu-id="ac539-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ac539-103">Si vous recevez ce message, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ac539-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ac539-104">Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Office.</span><span class="sxs-lookup"><span data-stu-id="ac539-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ac539-105">Consultez la rubrique [URL et plages d’adresses IP Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ac539-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ac539-106">Accédez à **Démarrer** > l'**exécution**, puis tapez **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="ac539-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ac539-107">Assurez-vous que les services suivants sont en cours d’exécution :</span><span class="sxs-lookup"><span data-stu-id="ac539-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ac539-108">Configuration automatique des périphériques connectés au réseau</span><span class="sxs-lookup"><span data-stu-id="ac539-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ac539-109">Service de liste de réseaux</span><span class="sxs-lookup"><span data-stu-id="ac539-109">Network List Service</span></span>
    - <span data-ttu-id="ac539-110">Connaissance des emplacements réseau</span><span class="sxs-lookup"><span data-stu-id="ac539-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ac539-111">Windows Journal des événements</span><span class="sxs-lookup"><span data-stu-id="ac539-111">Windows Event Log</span></span>

<span data-ttu-id="ac539-112">Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer.</span><span class="sxs-lookup"><span data-stu-id="ac539-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ac539-113">Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :</span><span class="sxs-lookup"><span data-stu-id="ac539-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ac539-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="ac539-114">**sfc /scannow**</span></span>

<span data-ttu-id="ac539-115">Une fois que cette commande est terminée, redémarrez l’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="ac539-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ac539-116">Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Veuillez réessayer plus tard» lorsque vous activez Office à partir de Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ac539-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>