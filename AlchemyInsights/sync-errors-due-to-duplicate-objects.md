---
title: 902 (erreurs de synchronisation dues à des objets en double)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420876"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a87b9-102">Erreurs de synchronisation dues à des objets dupliqués</span><span class="sxs-lookup"><span data-stu-id="a87b9-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a87b9-103">L'un des messages d'erreur suivants peut s'afficher à la fin de la synchronisation d'annuaires:</span><span class="sxs-lookup"><span data-stu-id="a87b9-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="a87b9-104">Impossible de mettre à jour cet objet dans Microsoft Online Services, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associées à un autre objet dans votre répertoire local.</span><span class="sxs-lookup"><span data-stu-id="a87b9-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="a87b9-105">Un objet synchronisé avec la même adresse proxy existe déjà dans votre répertoire Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="a87b9-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="a87b9-106">Impossible de mettre à jour cet objet car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans vos services d'annuaire local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a87b9-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="a87b9-107">Pour identifier et résoudre le problème, téléchargez et exécutez l' [outil de correction d'erreur DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="a87b9-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="a87b9-108">Pour plus d'informations, consultez la rubrique [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a87b9-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
