---
title: Procédure d’ajout ou de suppression d’un délégué dans Outlook pour Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571837"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="53d7b-102">Procédure d’ajout ou de suppression d’un délégué dans Outlook pour Windows</span><span class="sxs-lookup"><span data-stu-id="53d7b-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="53d7b-103">Pour ajouter un délégué dans Outlook pour Windows :</span><span class="sxs-lookup"><span data-stu-id="53d7b-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="53d7b-104">Cliquez sur l’onglet **fichier** , puis sur **paramètres du compte**, et choisissez **accès délégué**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="53d7b-105">Cliquez sur **Ajouter**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-105">Click on **Add**.</span></span> <span data-ttu-id="53d7b-106">Si **Ajouter** n’apparaît pas, il est possible qu’une connexion active n’existe pas entre Outlook et Exchange.</span><span class="sxs-lookup"><span data-stu-id="53d7b-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="53d7b-107">La barre d’État Outlook affiche l’état de la connexion.</span><span class="sxs-lookup"><span data-stu-id="53d7b-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="53d7b-108">Tapez le nom de la personne que vous voulez désigner comme délégué, ou recherchez et choisissez le nom dans la liste des résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="53d7b-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="53d7b-109">Le délégué doit être une personne figurant dans la liste d’adresses globale Exchange de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="53d7b-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="53d7b-110">Cliquez sur **Ajouter** , puis sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="53d7b-111">Dans la boîte de dialogue **autorisations des délégués** , acceptez les paramètres d’autorisation par défaut ou sélectionnez des niveaux d’accès personnalisés pour les dossiers Exchange.</span><span class="sxs-lookup"><span data-stu-id="53d7b-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="53d7b-112">Si un délégué a besoin de l’autorisation pour fonctionner uniquement avec des demandes de réunion et des réponses, les paramètres d’autorisation par défaut, tels que **Delegate, reçoivent une copie des messages relatifs à la réunion qui me** sont suffisants.</span><span class="sxs-lookup"><span data-stu-id="53d7b-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="53d7b-113">Vous pouvez laisser le paramètre autorisation de **boîte de réception** en **aucun**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="53d7b-114">Les demandes de réunion et les réponses seront directement envoyées vers la boîte de réception du délégué.</span><span class="sxs-lookup"><span data-stu-id="53d7b-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="53d7b-115">Par défaut, l’éditeur bénéficie de l’autorisation **éditeur (peut lire, créer et modifier des éléments)** sur votre dossier **calendrier** .</span><span class="sxs-lookup"><span data-stu-id="53d7b-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="53d7b-116">Lorsque le délégué répond à une réunion de votre part, il est automatiquement ajouté à votre dossier de **calendrier** .</span><span class="sxs-lookup"><span data-stu-id="53d7b-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="53d7b-117">Pour envoyer un message afin d’informer le délégué des autorisations modifiées, activez la case à cocher **Envoyer automatiquement un message au délégué pour résumer ces autorisations** .</span><span class="sxs-lookup"><span data-stu-id="53d7b-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="53d7b-118">Si vous le souhaitez, activez la case à cocher le **délégué peut voir mes éléments privés** .</span><span class="sxs-lookup"><span data-stu-id="53d7b-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="53d7b-119">Ce paramètre affecte tous les dossiers Exchange.</span><span class="sxs-lookup"><span data-stu-id="53d7b-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="53d7b-120">Cela inclut tous les dossiers courrier, contacts, calendrier, tâches, notes et journal.</span><span class="sxs-lookup"><span data-stu-id="53d7b-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="53d7b-121">Il n’existe aucun moyen d’accorder l’accès aux éléments privés dans les dossiers spécifiés uniquement.</span><span class="sxs-lookup"><span data-stu-id="53d7b-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="53d7b-122">Sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="53d7b-123">Les messages envoyés avec les autorisations Envoyer de la part de incluent les délégués et vos noms en regard **de**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="53d7b-124">Lorsqu’un message est envoyé avec les autorisations Envoyer en tant que, seul votre nom s’affiche.</span><span class="sxs-lookup"><span data-stu-id="53d7b-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="53d7b-125">Une fois que vous avez ajouté un utilisateur en tant que délégué, il peut ajouter votre boîte aux lettres Exchange à son profil Outlook.</span><span class="sxs-lookup"><span data-stu-id="53d7b-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="53d7b-126">Pour obtenir des instructions, consultez [la rubrique gérer les éléments de courrier et de calendrier d’une autre personne](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="53d7b-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="53d7b-127">Pour supprimer un délégué dans Outlook pour Windows :</span><span class="sxs-lookup"><span data-stu-id="53d7b-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="53d7b-128">Cliquez sur l’onglet **fichier** .</span><span class="sxs-lookup"><span data-stu-id="53d7b-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="53d7b-129">Cliquez sur **paramètres du compte** , puis sur **accès délégué**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="53d7b-130">Sélectionnez le nom du délégué pour lequel vous souhaitez modifier les autorisations, puis cliquez sur **supprimer** suivi de **OK**.</span><span class="sxs-lookup"><span data-stu-id="53d7b-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
