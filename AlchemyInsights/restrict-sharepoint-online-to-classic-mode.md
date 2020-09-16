---
title: Restreindre SharePoint Online au mode classique
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751420"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restreindre SharePoint Online au mode classique

Certaines organisations nécessitent toujours l’expérience en mode classique. Même s’il n’est pas prévu de supprimer le mode classique à un niveau granulaire, il n’est plus possible de limiter l’ensemble de l’organisation (client) au mode classique pour les listes et les bibliothèques.

Les options suivantes permettent aux administrateurs de gérer des listes et des bibliothèques individuelles en mode classique à l’aide de commutateurs d’exclusion granulaire que nous fournissons aux niveaux suivants :

- collection de sites
- site
- liste
- Bibliothèque

En outre, les listes qui utilisent certaines fonctionnalités et personnalisations qui ne sont pas prises en charge par Modern seront toujours automatiquement basculées vers le mode classique.

À partir du 1er avril 2019, le processus de désactivation de la liste et des bibliothèques modernes démarrera et continuera le 31 mai 2019.  Les listes et les bibliothèques en mode classique, à la suite de l’exclusion client, sont automatiquement déplacées vers la version moderne.

Si vous avez besoin du mode classique, reportez-vous à cette rubrique pour obtenir plus [d’informations et](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) des instructions PowerShell PNP [ici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) qui décrit les options et les outils que vous pouvez utiliser aujourd’hui pour utiliser l’expérience en mode classique.
