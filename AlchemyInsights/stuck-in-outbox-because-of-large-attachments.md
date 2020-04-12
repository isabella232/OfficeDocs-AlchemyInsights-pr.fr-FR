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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232628"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="bff7e-102">Corriger les messages bloqués dans la boîte d’envoi</span><span class="sxs-lookup"><span data-stu-id="bff7e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="bff7e-103">Nous vous recommandons de commencer par exécuter le scénario [« je rencontre des problèmes lors de l’envoi, de la réception ou de la recherche de messages électroniques »](https://aka.ms/SaRA-OutlookSendReceive) à partir de l’outil de [support et de récupération Microsoft](https://diagnostics.office.com/#/) sur l’ordinateur affecté.</span><span class="sxs-lookup"><span data-stu-id="bff7e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="bff7e-104">Lorsqu’un message est bloqué dans votre boîte d’envoi, la cause la plus probable est une pièce jointe de grande taille ou l’option « envoyer immédiatement une fois connecté » n’est pas activée.</span><span class="sxs-lookup"><span data-stu-id="bff7e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="bff7e-105">**Supprimer la pièce jointe de grande taille**</span><span class="sxs-lookup"><span data-stu-id="bff7e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="bff7e-106"> > Cliquez **su\r\*\*\**travailler en mode hors connexion**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="bff7e-107">Dans le volet de navigation, cliquez sur **boîte d’envoi**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="bff7e-108">À partir de là, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="bff7e-108">From here, you can:</span></span> 
    - <span data-ttu-id="bff7e-109">Supprimez le message.</span><span class="sxs-lookup"><span data-stu-id="bff7e-109">Delete the message.</span></span> <span data-ttu-id="bff7e-110">Sélectionnez-le et cliquez sur **supprimer**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="bff7e-111">Faites glisser le message vers votre **dossier Brouillons**, double-cliquez pour ouvrir le message et supprimez la pièce jointe (cliquez dessus, puis cliquez sur **supprimer**).</span><span class="sxs-lookup"><span data-stu-id="bff7e-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="bff7e-112">Si une erreur indique que Outlook tente de transmettre le message, fermez Outlook.</span><span class="sxs-lookup"><span data-stu-id="bff7e-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="bff7e-113">La fermeture peut prendre quelques instants.</span><span class="sxs-lookup"><span data-stu-id="bff7e-113">It may take a few moments to exit.</span></span> <span data-ttu-id="bff7e-114">Si Outlook ne se ferme pas, appuyez sur **Ctrl + Alt + Suppr** , puis cliquez sur **Démarrer le gestionnaire des tâches**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="bff7e-115">Dans le gestionnaire des tâches, sélectionnez l’onglet **processus** , faites défiler vers le bas jusqu’à Outlook. exe, puis cliquez sur **terminer le processus**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="bff7e-116">Après avoir fermé Outlook, redémarrez Outlook et répétez les étapes 2-3.</span><span class="sxs-lookup"><span data-stu-id="bff7e-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="bff7e-117">Après avoir supprimé la pièce jointe **, cliquez sur** > **travailler en mode hors connexion** pour désélectionner le bouton et continuer à travailler en ligne.</span><span class="sxs-lookup"><span data-stu-id="bff7e-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="bff7e-118">Les messages sont également bloqués dans la boîte d’envoi lorsque vous cliquez sur **Envoyer**, mais vous n’êtes pas connecté.</span><span class="sxs-lookup"><span data-stu-id="bff7e-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="bff7e-119">Cliquez sur **Envoyer/recevoir** , puis examinez le bouton **travailler hors connexion** .</span><span class="sxs-lookup"><span data-stu-id="bff7e-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="bff7e-120">S’il est bleu, c’est que vous êtes déconnecté.</span><span class="sxs-lookup"><span data-stu-id="bff7e-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="bff7e-121">Cliquez dessus pour vous connecter (le bouton active le blanc), puis cliquez sur **envoyer tout**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="bff7e-122">**Activer l’envoi immédiat une fois connecté**</span><span class="sxs-lookup"><span data-stu-id="bff7e-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="bff7e-123">Sous l’onglet Fichier, cliquez sur **Options**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="bff7e-124">Dans la boîte de dialogue Options d’Outlook, cliquez sur **Options avancées**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="bff7e-125">Dans la section envoyer et recevoir, cliquez sur pour activer l' **envoi immédiat une fois connecté**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="bff7e-126">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="bff7e-126">Click **OK**.</span></span>
 
<span data-ttu-id="bff7e-127">Pour plus d’informations, reportez-vous à :</span><span class="sxs-lookup"><span data-stu-id="bff7e-127">For full details, see:</span></span>
- [<span data-ttu-id="bff7e-128">Vidéo : envoyer ou supprimer un e-mail bloqué</span><span class="sxs-lookup"><span data-stu-id="bff7e-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="bff7e-129">Le courrier électronique reste dans le dossier boîte d’envoi tant que vous n’avez pas lancé manuellement une opération d’envoi/réception dans Outlook</span><span class="sxs-lookup"><span data-stu-id="bff7e-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
