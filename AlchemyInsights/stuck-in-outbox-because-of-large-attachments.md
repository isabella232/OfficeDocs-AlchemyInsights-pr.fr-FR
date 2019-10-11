---
title: Bloqué dans la boîte d’envoi en raison de pièces jointes volumineuses
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441304"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="25cb6-102">Corriger les messages bloqués dans la boîte d’envoi</span><span class="sxs-lookup"><span data-stu-id="25cb6-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="25cb6-103">Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="25cb6-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="25cb6-104">Lorsqu’un message est bloqué dans votre boîte d’envoi, les causes les plus probables sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="25cb6-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="25cb6-105">Pièces jointes volumineuses.</span><span class="sxs-lookup"><span data-stu-id="25cb6-105">Large attachments.</span></span>
- <span data-ttu-id="25cb6-106">L’option **Envoyer immédiatement une fois connecté** n’est pas activée.</span><span class="sxs-lookup"><span data-stu-id="25cb6-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="25cb6-107">Pour supprimer des pièces jointes volumineuses :</span><span class="sxs-lookup"><span data-stu-id="25cb6-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="25cb6-108">Dans Outlook **, sélectionnez** > **travailler en mode hors connexion**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="25cb6-109">Dans le volet de navigation, sélectionnez **boîte d’envoi**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="25cb6-110">À partir de là, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="25cb6-110">From here, you can:</span></span> 
    - <span data-ttu-id="25cb6-111">Supprimez le message (sélectionnez-le, puis sélectionnez **supprimer**).</span><span class="sxs-lookup"><span data-stu-id="25cb6-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="25cb6-112">Faites glisser le message vers votre dossier Brouillons, double-cliquez dessus pour l’ouvrir, puis supprimez la pièce jointe sélectionnez-la, puis sélectionnez **supprimer**).</span><span class="sxs-lookup"><span data-stu-id="25cb6-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="25cb6-113">Si vous recevez une erreur indiquant qu’Outlook tente de transmettre le message, fermez Outlook.</span><span class="sxs-lookup"><span data-stu-id="25cb6-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="25cb6-114">La fermeture peut prendre quelques instants.</span><span class="sxs-lookup"><span data-stu-id="25cb6-114">It may take a few moments to exit.</span></span> <span data-ttu-id="25cb6-115">Si Outlook ne se ferme pas, appuyez sur CTRL + ALT + SUPPR et sélectionnez **Démarrer le gestionnaire des tâches**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="25cb6-116">Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe et sélectionnez **terminer le processus**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="25cb6-117">Après avoir fermé Outlook, redémarrez-le et répétez les étapes 2 et 3.</span><span class="sxs-lookup"><span data-stu-id="25cb6-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="25cb6-118">Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour reprendre votre travail en ligne.</span><span class="sxs-lookup"><span data-stu-id="25cb6-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="25cb6-119">Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté.</span><span class="sxs-lookup"><span data-stu-id="25cb6-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="25cb6-120">Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** .</span><span class="sxs-lookup"><span data-stu-id="25cb6-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="25cb6-121">S’il est bleu, c’est que vous êtes déconnecté.</span><span class="sxs-lookup"><span data-stu-id="25cb6-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="25cb6-122">Sélectionnez-le pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="25cb6-123">Pour activer l' **envoi immédiat une fois connecté**:</span><span class="sxs-lookup"><span data-stu-id="25cb6-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="25cb6-124">Sélectionnez \*\*\*\* > \*\*\*\* options >  de fichier-**avancé**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="25cb6-125">Dans la section **Envoyer et recevoir** , sélectionnez **Envoyer immédiatement une fois connecté**, puis choisissez **OK**.</span><span class="sxs-lookup"><span data-stu-id="25cb6-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="25cb6-126">Pour obtenir des informations complètes, voir :</span><span class="sxs-lookup"><span data-stu-id="25cb6-126">For full details see:</span></span>
- [<span data-ttu-id="25cb6-127">Vidéo : envoyer ou supprimer un e-mail bloqué</span><span class="sxs-lookup"><span data-stu-id="25cb6-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="25cb6-128">Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook</span><span class="sxs-lookup"><span data-stu-id="25cb6-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
