---
title: Exchange PowerShell et la dépréciation de l’authentification de base
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813470"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="9d0ff-102">Exchange PowerShell et la dépréciation de l’authentification de base</span><span class="sxs-lookup"><span data-stu-id="9d0ff-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="9d0ff-103">Pour obtenir les informations les plus récentes sur la connexion à Exchange Online PowerShell sans utiliser l’authentification de base, [veuillez cliquer ici](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="9d0ff-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="9d0ff-104">Le module PowerShell V2 n’utilise pas l’authentification de base.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="9d0ff-105">Veuillez noter que l’authentification de base doit rester activée sur l’ordinateur de votre client.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="9d0ff-106">Le nouveau module PowerShell V2 utilise l’authentification moderne pour établir la connexion permettant d’activer toutes les applets de commande V2 se basant sur REST.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="9d0ff-107">Outre les applets de commande V2, elle vous permet également d’accéder à applets de commande Remote PowerShell (RPS) plus anciennes nécessitant l’établissement d’une session PowerShell à distance.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="9d0ff-108">L’établissement d’une session RPS sur un ordinateur Windows nécessite l’activation de WinRM BasicAuth sur l’ordinateur client, même si le module utilise un mécanisme d’authentification moderne pour s’authentifier auprès du service.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="9d0ff-109">Le pipeline WinRM BasicAuth est utilisé pour transporter des jetons d’authentification modernes.</span><span class="sxs-lookup"><span data-stu-id="9d0ff-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="9d0ff-110">Si WinRM BasicAuth est désactivée sur l’ordinateur client, les nouvelles applets de commande V2 continueront de fonctionner (à la différence des applets de commande RPS plus anciennes).</span><span class="sxs-lookup"><span data-stu-id="9d0ff-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
