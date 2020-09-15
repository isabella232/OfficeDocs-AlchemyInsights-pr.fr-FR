---
title: Résolution des problèmes liés aux événements de courriers électroniques
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658732"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4be01-102">Résolution des problèmes liés aux événements de courriers électroniques</span><span class="sxs-lookup"><span data-stu-id="4be01-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4be01-103">Vérifiez que la fonctionnalité est activée pour la boîte aux lettres : **Get-EventsFromEmailConfiguration-Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="4be01-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4be01-104">Examinez ensuite les journaux « événements de la messagerie électronique » **Exporter-MailboxDiagnosticLogs <mailbox>-Composant TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4be01-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4be01-105">Dans les journaux « Événements provenant de la messagerie », recherchez le InternetMessageId correspondant à l’élément dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4be01-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4be01-106">La TrustScore détermine si l’élément est ajouté ou non.</span><span class="sxs-lookup"><span data-stu-id="4be01-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4be01-107">Les événements ne sont ajoutés que si TrustScore = « Approuvé ».</span><span class="sxs-lookup"><span data-stu-id="4be01-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4be01-108">La TrustScore est déterminée par les propriétés SPF, Dkim ou Dmarc, qui se trouvent dans l’en-tête du message.</span><span class="sxs-lookup"><span data-stu-id="4be01-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4be01-109">Pour afficher ces propriétés :</span><span class="sxs-lookup"><span data-stu-id="4be01-109">To view these properties:</span></span>

<span data-ttu-id="4be01-110">**Bureau Outlook**</span><span class="sxs-lookup"><span data-stu-id="4be01-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4be01-111">Ouvrir l’élément</span><span class="sxs-lookup"><span data-stu-id="4be01-111">Open the item</span></span>
- <span data-ttu-id="4be01-112">Fichier -> Propriétés -> en-têtes Internet</span><span class="sxs-lookup"><span data-stu-id="4be01-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4be01-113">ou</span><span class="sxs-lookup"><span data-stu-id="4be01-113">or</span></span>

<span data-ttu-id="4be01-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="4be01-114">**MFCMapi**</span></span>

- <span data-ttu-id="4be01-115">Accéder à l’élément dans la boîte de réception</span><span class="sxs-lookup"><span data-stu-id="4be01-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4be01-116">Rechercher PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4be01-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4be01-117">Ces propriétés sont déterminées et enregistrées pendant le transport et routage.</span><span class="sxs-lookup"><span data-stu-id="4be01-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4be01-118">Pour résoudre le problème, vous devrez peut-être suivre le support de transport relatif aux échecs dans SPF, DKIM et. ou DMARC.</span><span class="sxs-lookup"><span data-stu-id="4be01-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>