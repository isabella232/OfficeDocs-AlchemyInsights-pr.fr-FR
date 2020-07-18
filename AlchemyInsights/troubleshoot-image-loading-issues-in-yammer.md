---
title: Résoudre les problèmes de chargement d’images dans Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146771"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="e1cbd-102">Résoudre les problèmes de chargement d’images dans Yammer</span><span class="sxs-lookup"><span data-stu-id="e1cbd-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="e1cbd-103">Lorsque des problèmes liés aux photos et aperçus de fichiers sont détectés dans Yammer, résolvez les problèmes en vérifiant si le problème se produit pour tous les utilisateurs, s'il se produit sur les appareils mobiles et s'il est reproductible lors du chargement de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="e1cbd-104">**Problèmes de photo de profil**</span><span class="sxs-lookup"><span data-stu-id="e1cbd-104">**Profile photo issues**</span></span>  

<span data-ttu-id="e1cbd-105">Si les utilisateurs finaux se connectent à Yammer via Microsoft 365, ils doivent modifier leur profil, y compris leur photo de profil.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="e1cbd-106">Si les utilisateurs ne sont pas autorisés à effectuer des mises à jour de profil, un administrateur peut effectuer la mise à jour pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="e1cbd-107">Pour plus d’informations, voir [Afficher et mettre à jour votre profil dans Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="e1cbd-108">Pour plus d’informations sur la modification de profil, notamment les photos de profil, consultez [Modifier mon profil et paramètres Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="e1cbd-109">Les photos de profil mises à jour sont synchronisées différemment par rapport aux attributs de profil.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="e1cbd-110">Les utilisateurs doivent se connecter pour lancer la synchronisation de leur photo de profil.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="e1cbd-111">Pour plus d’informations, consultez la rubrique [Les images de profil utilisateur mises à jour dans Office 365 le sont-elles également dans Yammer ?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="e1cbd-112">Pour plus d’informations sur le cycle de vie des utilisateurs de Yammer, consultez l’article [Gérer les utilisateurs de Yammer tout au long de leur cycle de vie à partir d’Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="e1cbd-113">Pour plus d’informations sur le fonctionnement de la synchronisation de la photo de profil dans Microsoft 365, consultez l’article [Informations sur la synchronisation de la photo de profil dans Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="e1cbd-114">**Aperçus de documents et problèmes de miniatures**</span><span class="sxs-lookup"><span data-stu-id="e1cbd-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="e1cbd-115">Lors de la publication de fichiers ou d’images dans Yammer, des aperçus peuvent ne pas s’afficher pour les raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="e1cbd-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="e1cbd-116">Le fichier est endommagé et ne peut pas être traité.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="e1cbd-117">Le fichier n'a pas été récemment chargé sur SharePoint Online, ou Yammer contient des métadonnées non valides pour d'autres raisons.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="e1cbd-118">Les URL nécessaires au chargement des images d'aperçu sont bloquées.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="e1cbd-119">L’aperçu du fichier a été supprimé par l’utilisateur avant la publication.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="e1cbd-120">Un problème de service a empêché la génération d’aperçus.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="e1cbd-121">**Remarque** les aperçus des liens et des chargements de fichiers peuvent se comporter différemment.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="e1cbd-122">Il se peut que des liens vers des fichiers sur Internet ou des liens nécessitant une authentification supplémentaire ne s’affichent pas correctement.</span><span class="sxs-lookup"><span data-stu-id="e1cbd-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="e1cbd-123">Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Joindre un fichier ou une image à un message de Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="e1cbd-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 