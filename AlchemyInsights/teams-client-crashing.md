---
title: 'Le client Teams se bloque :'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826269"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a2f97-102">Le client Teams se bloque :</span><span class="sxs-lookup"><span data-stu-id="a2f97-102">Teams client crashing?</span></span>

<span data-ttu-id="a2f97-103">Si votre client Teams se bloque, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a2f97-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a2f97-104">Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a2f97-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a2f97-105">Assurez-vous que toutes les [plages d’adresses et d’URL Microsoft 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) sont accessibles.</span><span class="sxs-lookup"><span data-stu-id="a2f97-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a2f97-106">Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.</span><span class="sxs-lookup"><span data-stu-id="a2f97-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="a2f97-107">Désinstaller et réinstaller l’application Teams (lien)</span><span class="sxs-lookup"><span data-stu-id="a2f97-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="a2f97-108">Accédez au dossier %appdata%\Microsoft\teams\ sur votre ordinateur et supprimez tous les fichiers dans ce répertoire.</span><span class="sxs-lookup"><span data-stu-id="a2f97-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="a2f97-109">[Téléchargez et installez l’application Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)et, si possible, installez teams en tant qu’administrateur (cliquez avec le bouton droit sur le programme d’installation Teams, puis sélectionnez « Exécuter en tant qu’administrateur » si disponible).</span><span class="sxs-lookup"><span data-stu-id="a2f97-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="a2f97-110">Si votre client Teams ne fonctionne toujours pas, pouvez-vous reproduire le problème ?</span><span class="sxs-lookup"><span data-stu-id="a2f97-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="a2f97-111">Si c’est le cas :</span><span class="sxs-lookup"><span data-stu-id="a2f97-111">If so:</span></span>

1. <span data-ttu-id="a2f97-112">Utilisez l’Enregistreur d’actions pour capturer vos étapes.</span><span class="sxs-lookup"><span data-stu-id="a2f97-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="a2f97-113">Fermez TOUTES les applications superflues ou confidentielles.</span><span class="sxs-lookup"><span data-stu-id="a2f97-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="a2f97-114">Lancez l’Enregistreur d’actions et reproduisez le problème lors de la connexion avec le compte d’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="a2f97-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="a2f97-115">[Collecter les journaux des équipes qui capturent les étapes de reproduction enregistrées](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="a2f97-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="a2f97-116">**Remarque** : Veillez à capturer l’adresse de connexion de l’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="a2f97-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="a2f97-117">Collectez les informations de copie de sauvegarde et/ou de compartiment défectueux (Windows).</span><span class="sxs-lookup"><span data-stu-id="a2f97-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="a2f97-118">Lancez Windows PowerShell sur l’ordinateur sur lequel le blocage se produit et exécutez les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a2f97-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="a2f97-119">Joignez le fichier à votre cas de support.</span><span class="sxs-lookup"><span data-stu-id="a2f97-119">Attach the file to your support case.</span></span>
