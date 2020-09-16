---
title: 902 (erreurs de synchronisation dues à des objets en double)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737339"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="b4314-102">Erreurs de synchronisation dues à des objets dupliqués</span><span class="sxs-lookup"><span data-stu-id="b4314-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="b4314-103">Vous pouvez recevoir l’un des messages d’erreur suivants lorsque la synchronisation d’annuaires se termine dans Microsoft 365 :</span><span class="sxs-lookup"><span data-stu-id="b4314-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="b4314-104">Impossible de mettre à jour cet objet dans Microsoft Online Services, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associées à un autre objet dans votre répertoire local.</span><span class="sxs-lookup"><span data-stu-id="b4314-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="b4314-105">Un objet synchronisé avec la même adresse proxy existe déjà dans votre répertoire Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="b4314-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="b4314-106">Impossible de mettre à jour cet objet car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans vos services d’annuaire local : UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b4314-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="b4314-107">Pour identifier et résoudre le problème, téléchargez et exécutez l' [outil de correction d’erreur DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="b4314-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="b4314-108">Pour plus d’informations, consultez la rubrique [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="b4314-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
