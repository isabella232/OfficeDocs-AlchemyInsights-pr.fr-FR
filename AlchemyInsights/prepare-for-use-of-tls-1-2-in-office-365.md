---
title: Préparer l’utilisation de TLS 1.2 dans Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085902"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Préparer l’utilisation de TLS 1.2 dans Microsoft 365

En date du 31 octobre 2018, la transition de Microsoft 365 vers TLS 1.2 se poursuit. À compter du 15 octobre 2020, O365 commencera l’obsolescence de TLS 1.0 et 1.1 au sein du service. Le déploiement de cette modification se poursuivra au cours des semaines et des mois qui suivent, mais les clients doivent s’assurer qu’aucun appel TLS 1.0/1.1 ne sera en fonction lorsqu’ils commenceront à intervenir sur Office 365 à partir du 15 octobre 2020. Comme précédemment communiqué (MC126199 en décembre 2017, MC128929 en février 2018, MC186827 en juillet 2019 et MC218794 en juillet 2020), nous déplaçons tous nos services en ligne vers le protocole TLS (Transport Layer Security) 1.2+ afin d’offrir un niveau de chiffrement optimal et de garantir la sécurité de notre service, par défaut. Les clients peuvent choisir de disposer de TLS 1.0/1.1 sur leurs serveurs et ressources, mais ils doivent seulement supposer que le protocole TLS 1.2 ou version ultérieure fonctionnera lorsque vous interagissez avec des ressources Office 365.
  
Pour en savoir plus sur ces changements, consultez [ceci](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) et [cela](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  