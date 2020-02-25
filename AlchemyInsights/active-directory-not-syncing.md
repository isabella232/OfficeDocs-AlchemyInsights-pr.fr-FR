---
title: Active Directory n’est pas en cours de synchronisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265193"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="251ee-102">Active Directory n’est pas en cours de synchronisation</span><span class="sxs-lookup"><span data-stu-id="251ee-102">Active Directory not syncing</span></span>

<span data-ttu-id="251ee-103">Si vous recevez des erreurs de synchronisation, telles que « pas de synchronisation récente », ou Notez que l’état de synchronisation d’annuaires dans le portail d’administration Office indique « dernière synchronisation il y a plus de 3 jours », cela peut être que les paramètres de AADConnect sont incorrects ou insuffisants autorisations pour effectuer une synchronisation.</span><span class="sxs-lookup"><span data-stu-id="251ee-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="251ee-104">La réinstallation de AADConnect à l’aide des paramètres rapides peut résoudre le problème rapidement :</span><span class="sxs-lookup"><span data-stu-id="251ee-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="251ee-105">[Téléchargez la dernière version de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="251ee-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="251ee-106">[Suivez les instructions pour l’installation d’Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="251ee-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="251ee-107">Pour plus d’informations sur les comptes de service AADConnect, reportez-vous à la rubrique [Azure ad Connect : comptes et autorisations](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="251ee-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
