---
title: Outil de diagnostic de service pour Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: e6c20af2c3fc54b203f3bda5c0c0f00faacd92800566bd507867c4e9fe4a23f1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052312"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Outil de diagnostic de service pour Windows Virtual Desktop

Windows Virtual Desktop (WVD) offre un outil de diagnostic qui permet aux administrateurs d'identifier les erreurs par le biais d'une interface unique. Cet outil enregistre les informations relatives aux diagnostics chaque fois que l' UDS est utilisé par une personne à laquelle un rôle UDS a été attribué. Chaque journal contient des informations sur le rôle de l'UVE impliqué dans l'activité, les messages d'erreur qui apparaissent pendant la session, ainsi que des informations sur le locataire et l'utilisateur. Les analyses de journaux Azure peuvent être configurées pour capturer le journal d'activité créé par l'outil de diagnostic en suivant ces étapes :

1. Créez un espace de travail pour les analyses de journaux avec le [portail Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Connecter les ordinateurs Windows à Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenez l'ID de l'espace de travail et la clé primaire de votre espace de travail. L'assistant d'installation a besoin de ces informations pour configurer correctement l'agent et s'assurer qu'il peut communiquer avec Azure Monitor.

1. [Transférez les données de diagnostic dans votre espace de travail](https://go.microsoft.com/fwlink/?linkid=2128284). Vous pouvez pousser les données de diagnostic de votre locataire WVD vers les analyses de journaux de votre espace de travail.

1. [Identifier et diagnostiquer ](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)les problèmes internes ou externes liés à la DVG.

Pour en savoir plus sur la configuration de l'outil de diagnostic de service pour WVD, voir Utiliser l'analyse des journaux pour la fonction de diagnostic.