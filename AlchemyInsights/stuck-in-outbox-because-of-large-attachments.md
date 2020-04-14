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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241250"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="de60f-102">Corriger les messages bloqués dans la boîte d’envoi</span><span class="sxs-lookup"><span data-stu-id="de60f-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="de60f-103">Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="de60f-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="de60f-104">Lorsqu’un message est bloqué dans votre boîte d’envoi, la cause la plus probable est une pièce jointe de grande taille ou l’option « envoyer immédiatement une fois connecté » n’est pas activée.</span><span class="sxs-lookup"><span data-stu-id="de60f-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="de60f-105">**Supprimer la pièce jointe de grande taille**</span><span class="sxs-lookup"><span data-stu-id="de60f-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="de60f-106">Dans Outlook **, sélectionnez** > **travailler en mode hors connexion**.</span><span class="sxs-lookup"><span data-stu-id="de60f-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="de60f-107">Dans le volet de navigation, sélectionnez **boîte d’envoi**.</span><span class="sxs-lookup"><span data-stu-id="de60f-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="de60f-108">À partir de là, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="de60f-108">From here, you can:</span></span> 
    - <span data-ttu-id="de60f-109">Supprimez le message (sélectionnez-le, puis sélectionnez **supprimer**).</span><span class="sxs-lookup"><span data-stu-id="de60f-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="de60f-110">Faites glisser le message vers votre dossier Brouillons, double-cliquez dessus pour l’ouvrir, puis supprimez la pièce jointe sélectionnez-la, puis sélectionnez **supprimer**).</span><span class="sxs-lookup"><span data-stu-id="de60f-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="de60f-111">Si vous recevez une erreur indiquant qu’Outlook tente de transmettre le message, fermez Outlook.</span><span class="sxs-lookup"><span data-stu-id="de60f-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="de60f-112">La fermeture peut prendre quelques instants.</span><span class="sxs-lookup"><span data-stu-id="de60f-112">It may take a few moments to exit.</span></span> <span data-ttu-id="de60f-113">Si Outlook ne se ferme pas, appuyez sur CTRL + ALT + SUPPR et sélectionnez **Démarrer le gestionnaire des tâches**.</span><span class="sxs-lookup"><span data-stu-id="de60f-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="de60f-114">Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe et sélectionnez **terminer le processus**.</span><span class="sxs-lookup"><span data-stu-id="de60f-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="de60f-115">Après avoir fermé Outlook, redémarrez-le et répétez les étapes 2 et 3.</span><span class="sxs-lookup"><span data-stu-id="de60f-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="de60f-116">Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour reprendre votre travail en ligne.</span><span class="sxs-lookup"><span data-stu-id="de60f-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="de60f-117">Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté.</span><span class="sxs-lookup"><span data-stu-id="de60f-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="de60f-118">Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** .</span><span class="sxs-lookup"><span data-stu-id="de60f-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="de60f-119">S’il est bleu, c’est que vous êtes déconnecté.</span><span class="sxs-lookup"><span data-stu-id="de60f-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="de60f-120">Cliquez dessus pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.</span><span class="sxs-lookup"><span data-stu-id="de60f-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="de60f-121">**Activer l’envoi immédiat une fois connecté**</span><span class="sxs-lookup"><span data-stu-id="de60f-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="de60f-122">Sous l’onglet Fichier, cliquez sur **Options**.</span><span class="sxs-lookup"><span data-stu-id="de60f-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="de60f-123">Dans la boîte de dialogue Options d’Outlook, cliquez sur **Options avancées**.</span><span class="sxs-lookup"><span data-stu-id="de60f-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="de60f-124">Dans la section envoyer et recevoir, cliquez sur pour activer l' **envoi immédiat une fois connecté**.</span><span class="sxs-lookup"><span data-stu-id="de60f-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="de60f-125">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="de60f-125">Click **OK**.</span></span>
 
<span data-ttu-id="de60f-126">Pour plus d’informations, reportez-vous à :</span><span class="sxs-lookup"><span data-stu-id="de60f-126">For full details, see:</span></span>
- [<span data-ttu-id="de60f-127">Vidéo : envoyer ou supprimer un e-mail bloqué</span><span class="sxs-lookup"><span data-stu-id="de60f-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="de60f-128">Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook</span><span class="sxs-lookup"><span data-stu-id="de60f-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
