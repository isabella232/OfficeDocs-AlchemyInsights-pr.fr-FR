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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>DéPréciation des plages d'adresses IP sortantes EOP

Nous avons détecté un problème potentiel avec votre organisation, qui (si elle n'a pas été corrigé par le 26 octobre 2018) peut rompre le flux de messagerie vers vos destinations locales ou externes. Comme précédemment communiqué, pour simplifier la gestion des plages d'adresses IP, nous consolidons les plages d'adresses IP d'Exchange Online Protection (EOP) qui sont utilisées pour envoyer et recevoir des courriers électroniques en dehors d'Office 365. Notre analyse indique qu'une ou plusieurs des sources de messagerie ou des destinations externes que vous avez configurées dans les connecteurs de flux de messagerie n'acceptent pas les connexions à partir des plages d'adresses IP indiquées [ici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Act avant le 26 octobre pour s'assurer que ces sources et destinations acceptent les connexions vers et à partir de toutes les [adresses IP EOP publiées](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Pour plus d'informations sur cette modification, consultez la rubrique messages Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Remarque**: Si vous utilisiez précédemment la publication IP ou URL via html, XML et RSS pour les mises à jour de point de terminaison, vous devez également effectuer une migration vers les nouveaux services Web pour l'automatisation de ces types de mises à jour. Pour plus d'informations, consultez les [catégories de point de terminaison office 365 et l'adresse IP d'office 365 et le service Web d'URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

