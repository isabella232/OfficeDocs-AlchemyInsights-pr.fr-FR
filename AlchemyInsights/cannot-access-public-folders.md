---
title: Impossible d’accéder aux dossiers publics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959493"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="2a053-102">Outlook ne peut pas se connecter aux dossiers publics</span><span class="sxs-lookup"><span data-stu-id="2a053-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="2a053-103">Si l’accès aux dossiers publics ne fonctionne pas pour quelques utilisateurs, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="2a053-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="2a053-104">Connectez-vous à EXO PowerShell et configurez le DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde à un compte d’utilisateur en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="2a053-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="2a053-105">Exemple :</span><span class="sxs-lookup"><span data-stu-id="2a053-105">Example:</span></span>

<span data-ttu-id="2a053-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="2a053-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="2a053-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valeur de la commande précédente></span><span class="sxs-lookup"><span data-stu-id="2a053-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="2a053-108">Patientez au moins une heure pour que la modification prenne effet.</span><span class="sxs-lookup"><span data-stu-id="2a053-108">Wait at least one hour for the change to take effect.</span></span>