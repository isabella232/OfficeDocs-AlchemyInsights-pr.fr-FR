---
title: 902 (erreurs de synchronisation en raison de la duplication d’objets)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469285"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a2205-102">Erreurs de synchronisation en raison d’objets en double</span><span class="sxs-lookup"><span data-stu-id="a2205-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a2205-103">Vous pouvez recevoir un des messages d’erreur suivants lors de la fin de la synchronisation d’annuaires :</span><span class="sxs-lookup"><span data-stu-id="a2205-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="a2205-104">Impossible de mettre à jour de cet objet dans Microsoft Online Services, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associés à un autre objet dans votre répertoire local.</span><span class="sxs-lookup"><span data-stu-id="a2205-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="a2205-105">Un objet synchronisé avec la même adresse proxy existe déjà dans votre annuaire Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="a2205-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="a2205-106">Impossible de mettre à jour de cet objet, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associés à un autre objet dans vos services d’annuaire local : UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a2205-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="a2205-107">Pour identifier et résoudre le problème, téléchargez et exécutez l' [Outil de correction d’erreurs IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="a2205-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="a2205-108">Pour plus d’informations, voir [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a2205-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

