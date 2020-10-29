---
title: Connecteur Exchange sur site Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791421"
---
# <a name="intune-exchange-on-premise-connector"></a>Connecteur Exchange sur site Intune

Pour plus d’informations sur la configuration du connecteur entre Intune et Exchange hébergé en local, reportez-vous à la documentation suivante :

[Configurer le connecteur Exchange sur site Intune dans Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

Q : je reçois une erreur telle que « la version du connecteur Exchange n’est pas prise en charge » lorsque vous tentez de configurer le connecteur Exchange. Quelle peut être la cause ?

A : le compte que vous utilisez dispose d’une licence Intune active.

Q : est-il possible d’avoir plusieurs connecteurs Exchange ?

A : vous ne pouvez configurer qu’un connecteur Exchange par client Intune par organisation Exchange. Le connecteur ne peut être installé que sur un seul serveur dans une organisation Exchange multiserveur.

Vous ne pouvez pas non plus configurer des connecteurs pour Exchange sur site et Exchange Online configurés dans le même client.

Q : le connecteur peut-il utiliser un tableau CAS comme connexion à Exchange ?

A : la spécification d’un tableau CAS n’est pas une configuration prise en charge dans le programme d’installation du connecteur. Seul un seul serveur doit être spécifié et doit être codé en dur dans le fichier de configuration du connecteur, qui se trouve dans

Program Data\Microsoft\Microsoft Intune sur site connecteur Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Recherchez l’entrée suivante ```<ExchangeWebServiceURL />``` et remplacez l’URL par le serveur Exchange.

**Tels**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Consultez la documentation suivante pour plus d’informations sur la résolution des problèmes : [dépanner le connecteur Exchange Intune sur site](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Activation de la journalisation détaillée pour le connecteur Exchange**

1. Ouvrez le fichier de configuration de suivi du connecteur Exchange pour le modifier.  
Le fichier se trouve à l’emplacement suivant :%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Tels**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Recherchez le TraceSourceLine avec la clé suivante : OnPremisesExchangeConnectorService  
  
3. Modifiez la valeur du nœud SourceLevel à partir de ActivityTracing d’informations (valeur par défaut) en verbose ActivityTracing  

**Exemple :**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Redémarrer le service Exchange Microsoft Intune  
5. Synchronisation complète dans le portail Intune jusqu’à ce qu’il se termine, puis redéfinissez le XML sur « information ActivityTracing » et redémarrez le service Exchange Microsoft Intune.  
6. L’emplacement des journaux est le suivant : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`