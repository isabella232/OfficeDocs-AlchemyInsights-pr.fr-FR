---
title: 1332 OWA - règles de boîte de réception n’exécutent pas pour une boîte aux lettres
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915802"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="dba72-102">Une règle de boîte de réception ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="dba72-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="dba72-103">Vérifiez les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="dba72-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="dba72-p101">Un message peut être redirigé, transféré ou réponses automatiquement en fonction des règles de boîte de réception qu’une seule fois. Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également connu sous le nom d’une règle de transport) permettre ajouter un maximum de 10 des destinataires de transfert d’un message. Pour plus d’informations, voir [limites de règle de Journal, de Transport et de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="dba72-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="dba72-p102">Règles de boîte de réception ne fonctionnent pas sur la boîte aux lettres de journalisation de substitution. Pour plus d’informations sur la boîte aux lettres de journalisation de substitution, voir [boîtes aux lettres de journalisation de substitution](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="dba72-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="dba72-109">Pour résoudre ces problèmes, consultez la rubrique [2829319 Ko](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="dba72-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="dba72-110">Si les problèmes précédents ne s’appliquent pas, exécutez le rapport de diagnostic de règle de boîte de réception avant de résoudre le problème au Support Microsoft :</span><span class="sxs-lookup"><span data-stu-id="dba72-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="dba72-111">Ouvrez la boîte aux lettres dans Outlook sur le web, puis cliquez sur **paramètres** \> **Options** \> **e-mail organiser** \> **les règles de boîte de réception**.</span><span class="sxs-lookup"><span data-stu-id="dba72-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="dba72-112">En bas de la page, cliquez sur **Si vos règles ne fonctionnent pas cliquer ici pour générer un rapport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="dba72-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

