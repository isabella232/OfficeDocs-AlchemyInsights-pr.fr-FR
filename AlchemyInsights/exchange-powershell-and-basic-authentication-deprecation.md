---
title: Exchange PowerShell et la dépréciation de l’authentification de base
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015687"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="f86e7-102">Exchange PowerShell et la dépréciation de l’authentification de base</span><span class="sxs-lookup"><span data-stu-id="f86e7-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="f86e7-103">Pour obtenir les informations les plus récentes sur la connexion à Exchange Online PowerShell sans utiliser l’authentification de base, [veuillez cliquer ici](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="f86e7-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="f86e7-104">Veuillez noter que l’authentification de base doit rester activée sur l’ordinateur de votre client.</span><span class="sxs-lookup"><span data-stu-id="f86e7-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="f86e7-105">Le nouveau module PowerShell V2 utilise l’authentification moderne pour établir la connexion permettant d’activer toutes les applets de commande V2 se basant sur REST.</span><span class="sxs-lookup"><span data-stu-id="f86e7-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="f86e7-106">Outre les applets de commande V2, elle vous permet également d’accéder à applets de commande Remote PowerShell (RPS) plus anciennes nécessitant l’établissement d’une session PowerShell à distance.</span><span class="sxs-lookup"><span data-stu-id="f86e7-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="f86e7-107">L’établissement d’une session RPS sur un ordinateur Windows nécessite l’activation de WinRM BasicAuth sur l’ordinateur client, même si le module utilise un mécanisme d’authentification moderne pour s’authentifier auprès du service.</span><span class="sxs-lookup"><span data-stu-id="f86e7-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="f86e7-108">Le pipeline WinRM BasicAuth est utilisé pour transporter des jetons d’authentification modernes.</span><span class="sxs-lookup"><span data-stu-id="f86e7-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="f86e7-109">Si WinRM BasicAuth est désactivée sur l’ordinateur client, les nouvelles applets de commande V2 continueront de fonctionner (à la différence des applets de commande RPS plus anciennes).</span><span class="sxs-lookup"><span data-stu-id="f86e7-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
