---
title: 'Le client Teams se bloque :'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: c49dfbf422b312f4744711d5f12b0eb83b6ebf2e
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44268770"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e629f-102">Le client Teams se bloque :</span><span class="sxs-lookup"><span data-stu-id="e629f-102">Teams client crashing?</span></span>

<span data-ttu-id="e629f-103">Si votre client Teams se bloque, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="e629f-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e629f-104">Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e629f-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e629f-105">Assurez-vous que toutes les [plages d’adresses et d’URL Microsoft 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) sont accessibles.</span><span class="sxs-lookup"><span data-stu-id="e629f-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e629f-106">Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.</span><span class="sxs-lookup"><span data-stu-id="e629f-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="e629f-107">Pour terminer, vous pouvez essayer de vider le cache de votre client Teams :</span><span class="sxs-lookup"><span data-stu-id="e629f-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="e629f-108">Quittez complètement le client de bureau Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e629f-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="e629f-109">Vous pouvez cliquer avec le bouton droit sur **Teams** à partir de Icon Tray, puis cliquez sur **Quitter** ou exécutez le Gestionnaire des tâches et terminez complètement le processus.</span><span class="sxs-lookup"><span data-stu-id="e629f-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="e629f-110">Accédez à l’Explorateur de fichiers, puis tapez %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="e629f-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="e629f-111">Une fois que vous êtes dans l’annuaire, quelques-uns des dossiers suivants s’affichent :</span><span class="sxs-lookup"><span data-stu-id="e629f-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="e629f-112">Dans **Application Cache**, accédez à Cache et supprimez les fichiers dans l’emplacement du Cache : %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="e629f-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="e629f-113">Dans **Blob_storage**, supprimez tous les fichiers : %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="e629f-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="e629f-114">Dans **Cache**, supprimez tous les fichiers : %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="e629f-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="e629f-115">Dans **databases**, supprimez tous les fichiers : %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="e629f-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="e629f-116">Dans **GPUCache**, supprimez tous les fichiers : %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="e629f-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="e629f-117">Dans **IndexedDB**, supprimez le fichier .db : %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="e629f-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="e629f-118">Dans **Local Stockage**, supprimez tous les fichiers : %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="e629f-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="e629f-119">Enfin, dans **tmp**, supprimez les fichiers suivants : %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="e629f-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="e629f-120">Redémarrez le client Teams.</span><span class="sxs-lookup"><span data-stu-id="e629f-120">Restart your Teams client.</span></span>

<span data-ttu-id="e629f-121">Si votre client Teams ne fonctionne toujours pas, pouvez-vous reproduire le problème ?</span><span class="sxs-lookup"><span data-stu-id="e629f-121">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="e629f-122">Si c’est le cas :</span><span class="sxs-lookup"><span data-stu-id="e629f-122">If so:</span></span> 

1. <span data-ttu-id="e629f-123">Utilisez l’Enregistreur d’actions pour capturer vos étapes.</span><span class="sxs-lookup"><span data-stu-id="e629f-123">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e629f-124">Fermez TOUTES les applications superflues ou confidentielles.</span><span class="sxs-lookup"><span data-stu-id="e629f-124">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e629f-125">Lancez l’Enregistreur d’actions et reproduisez le problème lors de la connexion avec le compte d’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="e629f-125">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    
2. <span data-ttu-id="e629f-126">Joignez le fichier à votre cas de support.</span><span class="sxs-lookup"><span data-stu-id="e629f-126">Attach the file to your support case.</span></span>
