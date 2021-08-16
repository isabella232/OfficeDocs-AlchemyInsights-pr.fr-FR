---
title: Intune Exchange connecteur local
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013962"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange connecteur local

Pour plus d’informations sur la configuration du connecteur entre Intune et Exchange qui est hébergé en local, consultez la documentation suivante :

[Configurer le connecteur d’Exchange Intune dans Azure Microsoft Intune](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

Q : Je vois une erreur telle que « La version du connecteur Exchange n’est pas prise en charge » lors de la tentative de Exchange connecteur. Quelle peut être la cause ?

R : Le compte que vous utilisez est titulaire d’une licence appropriée : il doit avoir une licence Intune active

Q : Est-il possible d’avoir plusieurs connecteurs Exchange réseau ?

R : Vous ne pouvez configurer qu’un connecteur Exchange par client Intune par Exchange organisation. Le connecteur ne peut être installé que sur un seul serveur dans une organisation Exchange à plusieurs serveurs.

En outre, vous ne pouvez pas avoir de connecteurs configurés pour Exchange sur site et Exchange Online configurés dans le même client.

Q : Le connecteur peut-il utiliser un tableau CAS comme connexion à Exchange ?

R : La spécification d’un tableau CAS n’est pas une configuration prise en charge dans la configuration du connecteur. Un seul serveur doit être spécifié et doit être codé en dur dans le fichier de configuration du connecteur qui se trouve dans

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Recherchez l’entrée suivante ```<ExchangeWebServiceURL />``` et remplacez l’URL par le serveur Exchange.

**Exemple :**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Pour plus de dépannage, consultez la documentation suivante : Dépannage du connecteur d’Exchange [Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Activation de la journalisation détaillée pour le connecteur Exchange de connexion**

1. Ouvrez le fichier Exchange configuration du suivi du connecteur pour le modifier.  
Le fichier se trouve à l’emplacement : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Exemple :**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Recherchez TraceSourceLine avec la clé suivante : OnPremisesExchangeConnectorService  
  
3. Modifier la valeur du nœud SourceLevel de Information ActivityTracing (valeur par défaut) à Verbose ActivityTracing  

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
4. Redémarrer le service Microsoft Intune Exchange service  
5. Synchronisation complète dans le portail Intune jusqu’à ce qu’il se termine, puis modifiez le XML en « Information ActivityTracing » et redémarrez le service Microsoft Intune Exchange service.  
6. L’emplacement des journaux est : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`