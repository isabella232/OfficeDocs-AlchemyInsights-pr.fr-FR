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
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784340"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Une règle de boîte de réception ne fonctionne pas comme prévu

Vérifiez les paramètres suivants:
  
- Un message peut être redirigé, transféré ou une réponse est automatiquement basée sur les règles de boîte de réception une seule fois. Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également appelée règle de transport) peut ajouter un maximum de dix destinataires de transfert à un message. Pour plus d'informations, consultez les [limitations de journal, de transport et de règles de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Les règles de boîte de réception ne fonctionnent pas sur l'autre boîte aux lettres de journalisation. Pour plus d'informations sur l'autre boîte aux lettres de journalisation, voir [autre boîte aux lettres](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)de journalisation.
    
Pour résoudre ces problèmes, reportez-vous à la rubrique [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Si les problèmes précédents ne s'appliquent pas, exécutez le rapport de diagnostic des règles de boîte de réception avant de remonter le problème vers le support Microsoft:
  
1. Ouvrez la boîte aux lettres dans Outlook sur le Web, puis cliquez sur **options** \> des **paramètres** \> organiser les **règles de boîte de réception**de **messagerie** \> .
    
2. Au bas de la page, cliquez sur **si vos règles ne fonctionnent pas cliquez ici pour générer un rapport de diagnostic**.
    

