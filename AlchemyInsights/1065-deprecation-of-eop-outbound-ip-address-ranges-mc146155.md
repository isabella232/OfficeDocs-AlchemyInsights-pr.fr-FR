---
title: 1065 désapprobation de EOP sortant IP adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934882"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="4d2f3-102">Désapprobation de plages d’adresses IP sortants EOP</span><span class="sxs-lookup"><span data-stu-id="4d2f3-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="4d2f3-p101">Nous avons détecté un problème avec votre organisation qui (si non résolues par le 26 octobre 2018) peuvent s’interrompre le flux de messagerie à votre localement ou à des destinations externes. Précédemment communiquée, pour simplifier la gestion de plage adresse IP, nous allons consolidation des plages d’adresses IP d’Exchange Online Protection (EOP) qui sont utilisés pour envoyer et recevoir du courrier électronique en dehors d’Office 365. Notre analyse indique qu’une ou plusieurs des sources de messagerie externe ou destinations que vous avez configurée dans les connecteurs de flux de messagerie ne sont pas accepter les connexions de l’IP adresse plages indiqué [ici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="4d2f3-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="4d2f3-106">Agir avant le 26 octobre afin de que ces sources et les destinations accepte les connexions vers et à partir de tous les [publié des adresses IP EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="4d2f3-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="4d2f3-107">Pour plus d’informations sur cette modification, consultez que le centre de messages billets [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="4d2f3-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="4d2f3-p102">**Remarque**: Si vous avez utilisé précédemment publication IP ou l’URL par HTML, XML et RSS pour les mises à jour du point de terminaison, vous également devez migrer vers les nouveaux services web pour l’automatisation de ces types de mises à jour. Pour plus d’informations, voir les [catégories de point de terminaison Office 365 et Office 365 adresse et URL service web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="4d2f3-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

