---
title: Libérer de l’espace disque dans Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897853"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="fbf59-102">Libérer de l’espace disque dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="fbf59-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="fbf59-103">Deux options s’offrent à vous pour libérer de l’espace sur le lecteur dans Windows :</span><span class="sxs-lookup"><span data-stu-id="fbf59-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="fbf59-104">Libérer de l’espace disque dans Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fbf59-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="fbf59-105">Libérez de l’espace pour les mises à jour Windows 10 avec un périphérique de stockage externe.</span><span class="sxs-lookup"><span data-stu-id="fbf59-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="fbf59-106">Si vous disposez toujours d'un faible espace disque après avoir utilisé le nettoyage de disque, il est possible que votre dossier Temp se remplisse rapidement de fichiers d'application (.appx) utilisés par Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="fbf59-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="fbf59-107">Pour résoudre ce problème, réinitialisez le Store, effacez le cache du Store, puis exécutez l'outil de résolution des problèmes de Windows Update.</span><span class="sxs-lookup"><span data-stu-id="fbf59-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="fbf59-108">Avant de procéder, assurez-vous que Microsoft Store est fermé.</span><span class="sxs-lookup"><span data-stu-id="fbf59-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="fbf59-109">**Étape 1 : réinitialiser Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="fbf59-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="fbf59-110">**Remarque** cette application supprime définitivement les données de l’application sur l’appareil, y compris vos préférences et les détails de la connectez-vous.</span><span class="sxs-lookup"><span data-stu-id="fbf59-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="fbf59-111">Sélectionnez **Démarrer** > **Paramètres** > **Applications** > **Applications et fonctionnalités**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="fbf59-112">Dans la liste des applications, recherchez et sélectionnez Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="fbf59-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="fbf59-113">Sélectionnez **Options avancées**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="fbf59-114">Faites défiler vers le bas et sélectionnez **Réinitialiser**, puis **Confirmer la réinitialisation**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="fbf59-115">**Étape 2 : effacer le cache du Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="fbf59-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="fbf59-116">Appuyez sur la touche de logo Windows+R pour ouvrir la boîte de dialogue Exécuter.</span><span class="sxs-lookup"><span data-stu-id="fbf59-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="fbf59-117">Tapez wsreset.exe, puis sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="fbf59-118">Une fenêtre d’invite de commandes vide s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="fbf59-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="fbf59-119">Après environ 10 secondes, la fenêtre se ferme et le Store s’ouvre automatiquement.</span><span class="sxs-lookup"><span data-stu-id="fbf59-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="fbf59-120">**Étape 3 : réinitialiser Windows Update**</span><span class="sxs-lookup"><span data-stu-id="fbf59-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="fbf59-121">Sélectionnez **Démarrer** > **Paramètres** > **Mise à jour et sécurité,** > **Résoudre des problèmes**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="fbf59-122">Faites défiler vers le bas et sélectionnez **Windows Update** dans la liste, puis sélectionnez **Exécuter l’utilitaire de résolution des problèmes**.</span><span class="sxs-lookup"><span data-stu-id="fbf59-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="fbf59-123">Redémarrez votre ordinateur et vérifiez que vous rencontrez toujours le problème.</span><span class="sxs-lookup"><span data-stu-id="fbf59-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

