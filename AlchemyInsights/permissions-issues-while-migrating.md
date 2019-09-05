---
title: Problèmes d’autorisations lors de la migration
ms.author: pebaum
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 33e605ff3019f52bbd0be876d485ff389b260a44
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752606"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="7fdb6-102">Synchronisation des profils utilisateur et des photos</span><span class="sxs-lookup"><span data-stu-id="7fdb6-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="7fdb6-103">**Synchronisation de photos de profil** : les utilisateurs peuvent remarquer que leur photo de profil n’est pas synchronisée avec SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="7fdb6-104">Ou bien, ils ont peut-être essayé de mettre à jour leur photo de profil et la photo apparaît toujours comme l’ancienne photo.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="7fdb6-105">Pour vous assurer que la photo de profil se présente comme prévu, l’utilisateur doit lancer une synchronisation des photos.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="7fdb6-106">Pour plus d’informations sur le processus de synchronisation des photos, voir [informations sur la synchronisation des images de profil dans Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="7fdb6-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="7fdb6-107">**Synchronisation des profils** : le temps nécessaire pour effectuer une synchronisation des profils dépend du nombre de modifications (travail) que le travail d’importation ad doit traiter.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="7fdb6-108">S’il existe de nombreuses modifications, le travail du minuteur a beaucoup de travail à effectuer, et les modifications apportées seront plus longues pour que les modifications soient reflétées dans l’application de profil utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="7fdb6-109">Si le travail du minuteur a un petit volume de travail à effectuer, les modifications seront beaucoup plus rapides dans l’application de profil utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="7fdb6-110">Pour plus d’informations sur le processus de synchronisation des profils, voir [informations sur la synchronisation des profils utilisateur dans SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639) .</span><span class="sxs-lookup"><span data-stu-id="7fdb6-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="7fdb6-111">**Mettre à jour le profil dans Office Delve** -Delve les utilisateurs peuvent gérer leur profil Office 365.</span><span class="sxs-lookup"><span data-stu-id="7fdb6-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="7fdb6-112">Pour plus d’informations, consultez [la rubrique afficher et mettre à jour votre profil dans Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="7fdb6-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

