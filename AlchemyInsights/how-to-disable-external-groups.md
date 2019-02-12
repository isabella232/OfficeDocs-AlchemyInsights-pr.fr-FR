---
title: Comment faire pour désactiver les groupes externes
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899134"
---
# <a name="how-to-disable-external-groups"></a>Comment faire pour désactiver les groupes externes

Yammer de messagerie externe s’applique les règles de Transport Exchange (ETRs), un ensemble de contrôles proactives pour empêcher les informations sur la société d’être partagé. Afin d’empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer pour la règle de Transport Exchange permet de bloquer la messagerie externe. 
  
Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer :
  
- Se connecter à Yammer comme un administrateur vérifié et dans **Centre d’administration de Yammer**, accédez à C **écurité et sécurité \> paramètres de sécurité.**
    
- Sous **Messagerie externe**, sélectionnez **appliquer votre Exchange Online règles de Transport Exchange (ETRs) dans Yammer.**
    
- Sélectionnez **Save (Enregistrer)**. 
    
Pour plus d’informations, consultez [contrôle externe de la messagerie dans un réseau Yammer avec des règles de Transport Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  

