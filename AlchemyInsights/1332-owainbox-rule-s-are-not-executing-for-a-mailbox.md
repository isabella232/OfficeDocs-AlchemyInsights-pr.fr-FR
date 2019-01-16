---
title: 1332 OWA - règles de boîte de réception n’exécutent pas pour une boîte aux lettres
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288609"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="85c08-102">Une règle de boîte de réception ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="85c08-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="85c08-103">Vérifiez les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="85c08-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="85c08-p101">Un message peut être redirigé, transféré ou réponses automatiquement en fonction des règles de boîte de réception qu’une seule fois. Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également connu sous le nom d’une règle de transport) permettre ajouter un maximum de 10 des destinataires de transfert d’un message. Pour plus d’informations, voir [limites de règle de Journal, de Transport et de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="85c08-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="85c08-p102">Règles de boîte de réception ne fonctionnent pas sur la boîte aux lettres de journalisation de substitution. Pour plus d’informations sur la boîte aux lettres de journalisation de substitution, voir [boîtes aux lettres de journalisation de substitution](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="85c08-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="85c08-109">Pour résoudre ces problèmes, consultez la rubrique [2829319 Ko](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="85c08-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="85c08-110">Si les problèmes précédents ne s’appliquent pas, exécutez le rapport de diagnostic de règle de boîte de réception avant de résoudre le problème au Support Microsoft :</span><span class="sxs-lookup"><span data-stu-id="85c08-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="85c08-111">Ouvrez la boîte aux lettres dans Outlook sur le web, puis cliquez sur **paramètres** \> **Options** \> **e-mail organiser** \> **les règles de boîte de réception**.</span><span class="sxs-lookup"><span data-stu-id="85c08-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="85c08-112">En bas de la page, cliquez sur **Si vos règles ne fonctionnent pas cliquer ici pour générer un rapport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="85c08-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

