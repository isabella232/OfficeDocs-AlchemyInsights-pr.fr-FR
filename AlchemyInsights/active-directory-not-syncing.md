---
title: Synchronisation d'Active Directory non
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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822849"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="1c79e-102">Synchronisation d'Active Directory non</span><span class="sxs-lookup"><span data-stu-id="1c79e-102">Active Directory not syncing</span></span>

<span data-ttu-id="1c79e-103">Si vous recevez des erreurs de synchronisation, telles que « aucune synchronisation récente », ou si vous remarquez que l'état de la synchronisation d'annuaires dans le portail d'administration Office indique « Dernière synchronisation il y a plus de 3 jours », il se peut qu'AADConnect dispose de paramètres incorrects ou d'autorisations insuffisantes pour effectuer une synchronisation.</span><span class="sxs-lookup"><span data-stu-id="1c79e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="1c79e-104">La réinstallation d'AADConnect à l'aide de paramètres express peut résoudre rapidement le problème :</span><span class="sxs-lookup"><span data-stu-id="1c79e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="1c79e-105">[Téléchargez la dernière version d'AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="1c79e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="1c79e-106">[Suivez les instructions pour l'installation rapide.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="1c79e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="1c79e-107">Pour plus d’informations sur les comptes de service AADConnect, consultez [Azure AD Connect : comptes et autorisations](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="1c79e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
