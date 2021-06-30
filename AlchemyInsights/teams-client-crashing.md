---
title: Blocage du client Teams
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187719"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e804a-102">Blocage du client Teams</span><span class="sxs-lookup"><span data-stu-id="e804a-102">Teams client crashing</span></span>

<span data-ttu-id="e804a-103">Si votre client Teams se bloque, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="e804a-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e804a-104">Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e804a-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e804a-105">Assurez-vous que toutes les [plages d’adresses et d’URL Microsoft 365 ](/microsoftteams/connectivity-issues) sont accessibles.</span><span class="sxs-lookup"><span data-stu-id="e804a-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e804a-106">Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.</span><span class="sxs-lookup"><span data-stu-id="e804a-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="e804a-107">Désinstaller et réinstaller l’application Teams</span><span class="sxs-lookup"><span data-stu-id="e804a-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="e804a-108">Accédez au dossier %appdata%\Microsoft\Teams\ sur votre ordinateur et supprimez tous les fichiers dans ce répertoire.</span><span class="sxs-lookup"><span data-stu-id="e804a-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="e804a-109">[Téléchargez et installez l’application Teams](https://www.microsoft.com/microsoft-teams/download-app)et, si possible, installez teams en tant qu’administrateur (cliquez avec le bouton droit sur le programme d’installation Teams, puis sélectionnez **Exécuter en tant qu’administrateur** si disponible).</span><span class="sxs-lookup"><span data-stu-id="e804a-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="e804a-110">Si votre client Teams se bloque toujours, essayez de reproduire le problème.</span><span class="sxs-lookup"><span data-stu-id="e804a-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="e804a-111">Si vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="e804a-111">If you can:</span></span>

1. <span data-ttu-id="e804a-112">Utilisez l’Enregistreur d’actions pour capturer vos étapes.</span><span class="sxs-lookup"><span data-stu-id="e804a-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e804a-113">Fermez TOUTES les applications superflues ou confidentielles.</span><span class="sxs-lookup"><span data-stu-id="e804a-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e804a-114">Lancez l’Enregistreur d’actions et reproduisez le problème lors de la connexion avec le compte d’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="e804a-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="e804a-115">[Collecter les journaux des équipes qui capturent les étapes de reproduction enregistrées](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="e804a-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="e804a-116">**Remarque** : Veillez à capturer l’adresse de connexion de l’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="e804a-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="e804a-117">Collectez les informations de copie de sauvegarde et/ou de compartiment défectueux (Windows).</span><span class="sxs-lookup"><span data-stu-id="e804a-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="e804a-118">Lancez Windows Powershell sur l’ordinateur sur lequel le blocage se produit et exécutez les commandes suivantes (après chaque commande, appuyez sur Entrée) :</span><span class="sxs-lookup"><span data-stu-id="e804a-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="e804a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="e804a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="e804a-120">Une fois le fichier texte généré et affiché à l’écran, enregistrez le fichier et attachez-le à la demande de service.</span><span class="sxs-lookup"><span data-stu-id="e804a-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
