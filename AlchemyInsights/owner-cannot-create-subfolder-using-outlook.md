---
title: Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716599"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="8850e-102">Le propriétaire ne peut pas créer un sous-dossier à l’aide d’Outlook</span><span class="sxs-lookup"><span data-stu-id="8850e-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="8850e-103">**Il y a un problème permanent lié aux propriétaires de dossiers publics qui créent des sous-dossiers à l’aide d’Outlook. Le problème sera prochainement résolu.**</span><span class="sxs-lookup"><span data-stu-id="8850e-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="8850e-104">En attendant, vous pouvez utiliser l'une des solutions de contournement suivantes :</span><span class="sxs-lookup"><span data-stu-id="8850e-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="8850e-105">Utiliser Outlook pour MAC pour créer le sous-dossier en tant que problème concernant uniquement Outlook pour Windows (toutes les versions)</span><span class="sxs-lookup"><span data-stu-id="8850e-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="8850e-106">Demandez à l’administrateur de créer le sous-dossier à l’aide de EXO Shell ou EAC</span><span class="sxs-lookup"><span data-stu-id="8850e-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="8850e-107">Remplacez DefaultPublicFolderMailbox/EffectivePublicFolderMailbox de l’utilisateur par une autre boîte aux lettres que la boîte aux lettres de contenu pour le dossier à l’origine du problème.</span><span class="sxs-lookup"><span data-stu-id="8850e-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="8850e-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="8850e-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="8850e-109">Patienter pendant une heure, redémarrez le client Outlook</span><span class="sxs-lookup"><span data-stu-id="8850e-109">Wait for an hour, restart outlook client</span></span>