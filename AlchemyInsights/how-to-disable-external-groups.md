---
title: Comment faire pour désactiver les groupes externes
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287900"
---
# <a name="how-to-disable-external-groups"></a>Comment faire pour désactiver les groupes externes

Yammer de messagerie externe s’applique les règles de Transport Exchange (ETRs), un ensemble de contrôles proactives pour empêcher les informations sur la société d’être partagé. Afin d’empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer pour la règle de Transport Exchange permet de bloquer la messagerie externe. 
  
Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer :
  
- Se connecter à Yammer comme un administrateur vérifié et dans **Centre d’administration de Yammer**, accédez à C **écurité et sécurité \> paramètres de sécurité.**
    
- Sous **Messagerie externe**, sélectionnez **appliquer votre Exchange Online règles de Transport Exchange (ETRs) dans Yammer.**
    
- Sélectionnez **Save (Enregistrer)**. 
    
Pour plus d’informations, consultez [contrôle externe de la messagerie dans un réseau Yammer avec des règles de Transport Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  

