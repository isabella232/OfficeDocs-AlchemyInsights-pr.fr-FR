---
title: Erreur d’adresse proxy lors de la création d’une boîte aux lettres partagée
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568288"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="a7d83-102">Erreur d’adresse proxy lors de la création d’une boîte aux lettres ou d’un autre objet à messagerie</span><span class="sxs-lookup"><span data-stu-id="a7d83-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="a7d83-103">Si vous avez essayé de créer un objet à messagerie (boîte aux lettres, boîte aux lettres partagée, etc.) et que vous avez reçu l’erreur « L’adresse proxy « SMTP:alias@domain.com » est déjà utilisée... », l’adresse de messagerie que vous avez choisie est déjà prise par un autre objet à messagerie dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="a7d83-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="a7d83-104">Vous devez rechercher l’utilisateur, le groupe, la boîte aux lettres partagée ou le dossier public qui possède cette adresse de messagerie et la supprimer ou modifier son adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="a7d83-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="a7d83-105">Vous pouvez ensuite créer un objet à messagerie avec l’adresse de messagerie libérée.</span><span class="sxs-lookup"><span data-stu-id="a7d83-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="a7d83-106">Utilisez la recherche sur la page d’accueil pour la rechercher.</span><span class="sxs-lookup"><span data-stu-id="a7d83-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="a7d83-107">Vous pouvez également utiliser la commande Exchange Online PowerShell suivante pour la rechercher :</span><span class="sxs-lookup"><span data-stu-id="a7d83-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="a7d83-108">Si vous ne souhaitez pas supprimer l’adresse de messagerie existante, choisissez une nouvelle adresse de messagerie pour le nouvel objet que vous créez.</span><span class="sxs-lookup"><span data-stu-id="a7d83-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  