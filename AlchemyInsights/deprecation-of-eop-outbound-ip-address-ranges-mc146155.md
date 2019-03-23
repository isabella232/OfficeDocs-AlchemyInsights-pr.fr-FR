---
title: 1065 déPréciation de l'adresse IP sortante rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777270"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="0e334-102">DéPréciation des plages d'adresses IP sortantes EOP</span><span class="sxs-lookup"><span data-stu-id="0e334-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="0e334-103">Nous avons détecté un problème potentiel avec votre organisation, qui (si elle n'a pas été corrigé par le 26 octobre 2018) peut rompre le flux de messagerie vers vos destinations locales ou externes.</span><span class="sxs-lookup"><span data-stu-id="0e334-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="0e334-104">Comme précédemment communiqué, pour simplifier la gestion des plages d'adresses IP, nous consolidons les plages d'adresses IP d'Exchange Online Protection (EOP) qui sont utilisées pour envoyer et recevoir des courriers électroniques en dehors d'Office 365.</span><span class="sxs-lookup"><span data-stu-id="0e334-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="0e334-105">Notre analyse indique qu'une ou plusieurs des sources de messagerie ou des destinations externes que vous avez configurées dans les connecteurs de flux de messagerie n'acceptent pas les connexions à partir des plages d'adresses IP indiquées [ici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0e334-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="0e334-106">Act avant le 26 octobre pour s'assurer que ces sources et destinations acceptent les connexions vers et à partir de toutes les [adresses IP EOP publiées](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0e334-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="0e334-107">Pour plus d'informations sur cette modification, consultez la rubrique messages Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="0e334-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="0e334-108">**Remarque**: Si vous utilisiez précédemment la publication IP ou URL via html, XML et RSS pour les mises à jour de point de terminaison, vous devez également effectuer une migration vers les nouveaux services Web pour l'automatisation de ces types de mises à jour.</span><span class="sxs-lookup"><span data-stu-id="0e334-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="0e334-109">Pour plus d'informations, consultez les [catégories de point de terminaison office 365 et l'adresse IP d'office 365 et le service Web d'URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="0e334-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

