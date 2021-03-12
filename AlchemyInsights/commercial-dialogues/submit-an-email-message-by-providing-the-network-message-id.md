---
title: Envoyer un message électronique en fournissant l’ID de message réseau
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735884"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="0feed-102">Envoyer un message électronique en fournissant l’ID de message réseau</span><span class="sxs-lookup"><span data-stu-id="0feed-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="0feed-103">Dans le **volant Nouvelle soumission,** sélectionnez **E-mail** et **ID de message réseau.**</span><span class="sxs-lookup"><span data-stu-id="0feed-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="0feed-104">Suivez ces étapes pour rechercher l’ID de message d’un message électronique dans Outlook :</span><span class="sxs-lookup"><span data-stu-id="0feed-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="0feed-105">Double-cliquez sur le message électronique pour l’ouvrir.</span><span class="sxs-lookup"><span data-stu-id="0feed-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="0feed-106">Sélectionnez **les**  >  **propriétés du fichier.**</span><span class="sxs-lookup"><span data-stu-id="0feed-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="0feed-107">Ouvrez le Bloc-notes ou un document Word vide, puis copiez et collez le contenu trouvé dans la zone d’en-tête **Internet** dans le document ouvert pour une meilleure visibilité.</span><span class="sxs-lookup"><span data-stu-id="0feed-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="0feed-108">Recherchez **le champ X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="0feed-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="0feed-109">La valeur après **:** est l’ID dont vous avez besoin pour votre soumission.</span><span class="sxs-lookup"><span data-stu-id="0feed-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="0feed-110">Sous **Destinataires**, si le courrier électronique a été envoyé dans le dossier courrier indésirable pour tous les destinataires de ce message, sélectionnez **Sélectionner tout.**</span><span class="sxs-lookup"><span data-stu-id="0feed-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="0feed-111">Si ce n’est pas le cas, sélectionnez uniquement l’utilisateur qui a signalé le problème.</span><span class="sxs-lookup"><span data-stu-id="0feed-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="0feed-112">Sous **Raison de l’envoi,** si vous sélectionnez Doit avoir été  **bloqué,** spécifiez si le message doit avoir été bloqué en tant que courrier **indésirable,** hameçonnage ou programme **malveillant,** puis sélectionnez **Envoyer.**</span><span class="sxs-lookup"><span data-stu-id="0feed-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="0feed-113">Pour plus d’informations, voir Comment soumettre des messages suspects de courrier indésirable, d’hameçonnage, d’URL et de fichiers [à Microsoft pour analyse.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="0feed-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
