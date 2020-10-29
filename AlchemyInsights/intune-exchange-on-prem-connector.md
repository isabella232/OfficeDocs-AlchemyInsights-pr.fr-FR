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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="a7a82-102">Connecteur Exchange sur site Intune</span><span class="sxs-lookup"><span data-stu-id="a7a82-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="a7a82-103">Pour plus d’informations sur la configuration du connecteur entre Intune et Exchange hébergé en local, reportez-vous à la documentation suivante :</span><span class="sxs-lookup"><span data-stu-id="a7a82-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="a7a82-104">Configurer le connecteur Exchange sur site Intune dans Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="a7a82-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="a7a82-105">**FAQ:**</span><span class="sxs-lookup"><span data-stu-id="a7a82-105">**FAQ:**</span></span>

<span data-ttu-id="a7a82-106">Q : je reçois une erreur telle que « la version du connecteur Exchange n’est pas prise en charge » lorsque vous tentez de configurer le connecteur Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a82-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="a7a82-107">Quelle peut être la cause ?</span><span class="sxs-lookup"><span data-stu-id="a7a82-107">What could be the cause?</span></span>

<span data-ttu-id="a7a82-108">A : le compte que vous utilisez dispose d’une licence Intune active.</span><span class="sxs-lookup"><span data-stu-id="a7a82-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="a7a82-109">Q : est-il possible d’avoir plusieurs connecteurs Exchange ?</span><span class="sxs-lookup"><span data-stu-id="a7a82-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="a7a82-110">A : vous ne pouvez configurer qu’un connecteur Exchange par client Intune par organisation Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a82-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="a7a82-111">Le connecteur ne peut être installé que sur un seul serveur dans une organisation Exchange multiserveur.</span><span class="sxs-lookup"><span data-stu-id="a7a82-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="a7a82-112">Vous ne pouvez pas non plus configurer des connecteurs pour Exchange sur site et Exchange Online configurés dans le même client.</span><span class="sxs-lookup"><span data-stu-id="a7a82-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="a7a82-113">Q : le connecteur peut-il utiliser un tableau CAS comme connexion à Exchange ?</span><span class="sxs-lookup"><span data-stu-id="a7a82-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="a7a82-114">A : la spécification d’un tableau CAS n’est pas une configuration prise en charge dans le programme d’installation du connecteur.</span><span class="sxs-lookup"><span data-stu-id="a7a82-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="a7a82-115">Seul un seul serveur doit être spécifié et doit être codé en dur dans le fichier de configuration du connecteur, qui se trouve dans</span><span class="sxs-lookup"><span data-stu-id="a7a82-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="a7a82-116">Program Data\Microsoft\Microsoft Intune sur site connecteur Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="a7a82-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="a7a82-117">Recherchez l’entrée suivante ```<ExchangeWebServiceURL />``` et remplacez l’URL par le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a82-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="a7a82-118">**Tels**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="a7a82-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="a7a82-119">Consultez la documentation suivante pour plus d’informations sur la résolution des problèmes : [dépanner le connecteur Exchange Intune sur site](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="a7a82-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="a7a82-120">**Activation de la journalisation détaillée pour le connecteur Exchange**</span><span class="sxs-lookup"><span data-stu-id="a7a82-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="a7a82-121">Ouvrez le fichier de configuration de suivi du connecteur Exchange pour le modifier.</span><span class="sxs-lookup"><span data-stu-id="a7a82-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="a7a82-122">Le fichier se trouve à l’emplacement suivant :%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="a7a82-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="a7a82-123">**Tels**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="a7a82-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="a7a82-124">Recherchez le TraceSourceLine avec la clé suivante : OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="a7a82-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="a7a82-125">Modifiez la valeur du nœud SourceLevel à partir de ActivityTracing d’informations (valeur par défaut) en verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="a7a82-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="a7a82-126">**Exemple :**</span><span class="sxs-lookup"><span data-stu-id="a7a82-126">**Example:**</span></span>
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
4. <span data-ttu-id="a7a82-127">Redémarrer le service Exchange Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a7a82-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="a7a82-128">Synchronisation complète dans le portail Intune jusqu’à ce qu’il se termine, puis redéfinissez le XML sur « information ActivityTracing » et redémarrez le service Exchange Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a7a82-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="a7a82-129">L’emplacement des journaux est le suivant : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="a7a82-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>