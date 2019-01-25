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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469255"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Une règle de boîte de réception ne fonctionne pas comme prévu

Vérifiez les paramètres suivants :
  
- Un message peut être redirigé, transféré ou réponses automatiquement en fonction des règles de boîte de réception qu’une seule fois. Une règle de redirection (une règle de boîte de réception ou une règle de flux de messagerie, également connu sous le nom d’une règle de transport) permettre ajouter un maximum de 10 des destinataires de transfert d’un message. Pour plus d’informations, voir [limites de règle de Journal, de Transport et de boîte de réception](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Règles de boîte de réception ne fonctionnent pas sur la boîte aux lettres de journalisation de substitution. Pour plus d’informations sur la boîte aux lettres de journalisation de substitution, voir [boîtes aux lettres de journalisation de substitution](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Pour résoudre ces problèmes, consultez la rubrique [2829319 Ko](https://support.microsoft.com/kb/2829319).
  
Si les problèmes précédents ne s’appliquent pas, exécutez le rapport de diagnostic de règle de boîte de réception avant de résoudre le problème au Support Microsoft :
  
1. Ouvrez la boîte aux lettres dans Outlook sur le web, puis cliquez sur **paramètres** \> **Options** \> **e-mail organiser** \> **les règles de boîte de réception**.
    
2. En bas de la page, cliquez sur **Si vos règles ne fonctionnent pas cliquer ici pour générer un rapport de diagnostic**.
    

