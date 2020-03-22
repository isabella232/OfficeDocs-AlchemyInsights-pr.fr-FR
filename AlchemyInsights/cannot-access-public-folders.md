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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891747"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="da9b1-102">Outlook ne peut pas se connecter aux dossiers publics</span><span class="sxs-lookup"><span data-stu-id="da9b1-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="da9b1-103">Si l’accès aux dossiers publics ne fonctionne pas pour certains utilisateurs, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="da9b1-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="da9b1-104">Connectez-vous à EXO PowerShell et configurez le paramètre DefaultPublicFolderMailbox sur le compte d’utilisateur posant problème pour qu’il corresponde au paramètre sur un compte d’utilisateur de travail.</span><span class="sxs-lookup"><span data-stu-id="da9b1-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="da9b1-105">Exemple :</span><span class="sxs-lookup"><span data-stu-id="da9b1-105">Example:</span></span>

<span data-ttu-id="da9b1-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="da9b1-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="da9b1-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valeur de la commande précédente></span><span class="sxs-lookup"><span data-stu-id="da9b1-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="da9b1-108">Patientez au moins une heure pour que la modification prenne effet.</span><span class="sxs-lookup"><span data-stu-id="da9b1-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="da9b1-109">Si le problème persiste, suivez [cette procédure](https://aka.ms/pfcte) pour résoudre les problèmes d’accès aux dossiers publics à l’aide d’Outlook.</span><span class="sxs-lookup"><span data-stu-id="da9b1-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>