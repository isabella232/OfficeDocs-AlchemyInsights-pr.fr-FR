---
title: 1065 Annulation des plages d’adresses IP sortantes EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031260"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Annulation des plages d’adresses IP sortantes EOP

Nous avons détecté un problème potentiel avec votre organisation qui (s’il n’est pas corrigé d’ici le 26 octobre 2018) pourrait rompre le flux de messagerie vers vos destinations sur site ou externes. Comme indiqué précédemment, pour simplifier la gestion des plages d’adresses IP, nous consolidons les plages d’adresses IP Exchange Online Protection (EOP) utilisées pour envoyer et recevoir des messages électroniques en dehors de Microsoft 365. Notre analyse indique qu’une ou plusieurs des sources ou destinations de messagerie externes que vous avez configurées dans les connecteurs de flux de messagerie n’acceptent pas les connexions des plages d’adresses IP indiquées [ici.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Agissez avant le 26 octobre pour vous assurer que ces sources et destinations accepteront les connexions vers et depuis toutes les [adresses IP EOP publiées.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Pour plus d’informations sur cette modification, consultez les billets du centre de messages [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ou [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Remarque**: si vous avez déjà utilisé la publication IP ou URL via HTML, XML et RSS pour les mises à jour de point de terminaison, vous devez également migrer vers les nouveaux services web pour automatiser ces types de mises à jour. Pour plus d’informations, voir Microsoft 365 catégories de point de terminaison et [Microsoft 365'adresse IP et le service web d’URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
