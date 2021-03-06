---
title: Recherche et suppression de messages électroniques dans votre organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500781"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="ec726-102">Recherche et suppression de messages électroniques dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="ec726-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="ec726-103">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ec726-103">Follow these steps:</span></span>

1. <span data-ttu-id="ec726-104">Si vous n’êtes pas un administrateur général, pour rechercher des messages, votre compte doit être ajouté au groupe de rôles Gestionnaire **eDiscovery** ou au rôle de gestion de la recherche de **conformité.**</span><span class="sxs-lookup"><span data-stu-id="ec726-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="ec726-105">Pour supprimer des messages, vous  devez rejoindre le groupe de rôles Gestion de l’organisation ou le rôle de gestion recherche **et purge.**</span><span class="sxs-lookup"><span data-stu-id="ec726-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="ec726-106">Les autorisations sur ces rôles sont attribuées dans le Centre de [sécurité & conformité.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="ec726-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="ec726-107">[Créez une recherche de](https://docs.microsoft.com/office365/securitycompliance/content-search) contenu pour rechercher le message à supprimer.</span><span class="sxs-lookup"><span data-stu-id="ec726-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="ec726-108">[Se connecter à l’interface PowerShell du Centre de sécurité et conformité](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ec726-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="ec726-109">Si vous utilisez l’authentification multifacteur, consultez les instructions suivantes : Se connecter au Centre de sécurité & conformité PowerShell à l’aide de [l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="ec726-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="ec726-110">Supprimez le message : exécutez `New-ComplianceSearchAction` la cmdlet pour supprimer le message.</span><span class="sxs-lookup"><span data-stu-id="ec726-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="ec726-111">Les messages supprimés sont déplacés vers le dossier Éléments récupérables d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ec726-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="ec726-112">Pour obtenir un exemple de commande, [voir Étape 3 : Supprimer le message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="ec726-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
