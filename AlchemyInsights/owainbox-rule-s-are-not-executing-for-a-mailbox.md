---
title: 1332 la ou les règles de boîte de réception OWA ne s'exécutent pas pour une boîte aux lettres
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858742"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5514a-102">Une règle de boîte de réception ne fonctionne pas comme prévu</span><span class="sxs-lookup"><span data-stu-id="5514a-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5514a-103">Vérifiez les paramètres suivants:</span><span class="sxs-lookup"><span data-stu-id="5514a-103">Verify the following settings:</span></span>

- <span data-ttu-id="5514a-104">Un message peut être redirigé, transféré ou une réponse est automatiquement basée sur les règles de boîte de réception une seule fois.</span><span class="sxs-lookup"><span data-stu-id="5514a-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5514a-105">Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également appelée règle de transport) peut ajouter un maximum de dix destinataires de transfert à un message.</span><span class="sxs-lookup"><span data-stu-id="5514a-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5514a-106">Pour plus d'informations, consultez les [limitations de journal, de transport et de règles de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="5514a-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5514a-107">Les règles de boîte de réception ne fonctionnent pas sur l'autre boîte aux lettres de journalisation.</span><span class="sxs-lookup"><span data-stu-id="5514a-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5514a-108">Pour plus d'informations sur l'autre boîte aux lettres de journalisation, voir [autre boîte aux lettres](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)de journalisation.</span><span class="sxs-lookup"><span data-stu-id="5514a-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5514a-109">Pour résoudre ces problèmes, reportez-vous à la rubrique [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="5514a-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5514a-110">Si les problèmes précédents ne s'appliquent pas, exécutez le rapport de diagnostic des règles de boîte de réception avant de remonter le problème vers le support Microsoft:</span><span class="sxs-lookup"><span data-stu-id="5514a-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5514a-111">Ouvrez la boîte aux lettres dans Outlook sur le Web, puis cliquez sur **options** \> des **paramètres** \> organiser les **règles de boîte de réception**de **messagerie** \> .</span><span class="sxs-lookup"><span data-stu-id="5514a-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="5514a-112">Au bas de la page, cliquez sur **si vos règles ne fonctionnent pas cliquez ici pour générer un rapport de diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="5514a-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
