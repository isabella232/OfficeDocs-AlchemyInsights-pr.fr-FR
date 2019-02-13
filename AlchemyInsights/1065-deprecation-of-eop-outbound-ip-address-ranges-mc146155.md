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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Désapprobation de plages d’adresses IP sortants EOP

Nous avons détecté un problème avec votre organisation qui (si non résolues par le 26 octobre 2018) peuvent s’interrompre le flux de messagerie à votre localement ou à des destinations externes. Précédemment communiquée, pour simplifier la gestion de plage adresse IP, nous allons consolidation des plages d’adresses IP d’Exchange Online Protection (EOP) qui sont utilisés pour envoyer et recevoir du courrier électronique en dehors d’Office 365. Notre analyse indique qu’une ou plusieurs des sources de messagerie externe ou destinations que vous avez configurée dans les connecteurs de flux de messagerie ne sont pas accepter les connexions de l’IP adresse plages indiqué [ici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Agir avant le 26 octobre afin de que ces sources et les destinations accepte les connexions vers et à partir de tous les [publié des adresses IP EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Pour plus d’informations sur cette modification, consultez que le centre de messages billets [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Remarque**: Si vous avez utilisé précédemment publication IP ou l’URL par HTML, XML et RSS pour les mises à jour du point de terminaison, vous également devez migrer vers les nouveaux services web pour l’automatisation de ces types de mises à jour. Pour plus d’informations, voir les [catégories de point de terminaison Office 365 et Office 365 adresse et URL service web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

