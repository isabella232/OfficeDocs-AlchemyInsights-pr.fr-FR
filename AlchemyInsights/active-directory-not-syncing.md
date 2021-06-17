---
title: Synchronisation d’Active Directory non
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930973"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="fbcd4-102">Synchronisation d’Active Directory non</span><span class="sxs-lookup"><span data-stu-id="fbcd4-102">Active Directory not syncing</span></span>

<span data-ttu-id="fbcd4-103">Si vous recevez des erreurs de synchronisation, telles que « aucune synchronisation récente », ou si vous remarquez que l’état de la synchronisation d’annuaires dans le portail d’administration Office indique « Dernière synchronisation il y a plus de 3 jours », il se peut qu’AADConnect dispose de paramètres incorrects ou d’autorisations insuffisantes pour effectuer une synchronisation.</span><span class="sxs-lookup"><span data-stu-id="fbcd4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="fbcd4-104">La réinstallation d’AADConnect à l’aide de paramètres express peut résoudre rapidement le problème :</span><span class="sxs-lookup"><span data-stu-id="fbcd4-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="fbcd4-105">[Téléchargez la dernière version d’AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="fbcd4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="fbcd4-106">[Suivez les instructions pour l’installation rapide.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="fbcd4-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="fbcd4-107">Azure AD Connect doit être installé sur Windows Server 2012 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="fbcd4-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="fbcd4-108">Ce serveur doit être joint au domaine et peut être un contrôleur de domaine ou un serveur membre.</span><span class="sxs-lookup"><span data-stu-id="fbcd4-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="fbcd4-109">Pour obtenir la liste complète des conditions requises et Connecter azure AD, examinez les conditions préalables pour [Azure AD Connecter](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span><span class="sxs-lookup"><span data-stu-id="fbcd4-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="fbcd4-110">Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="fbcd4-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
