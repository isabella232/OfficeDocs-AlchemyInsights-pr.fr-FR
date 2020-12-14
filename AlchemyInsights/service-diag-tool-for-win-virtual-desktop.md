---
title: Outil de diagnostic de service pour le bureau virtuel Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665817"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Outil de diagnostic de service pour le bureau virtuel Windows

Windows Virtual Desktop (WVD) propose un outil de diagnostic qui permet aux administrateurs d’identifier les erreurs via une seule interface. Cet outil enregistre les informations relatives aux diagnostics chaque fois que WVD est utilisé par une personne qui a un rôle WVD. Chaque journal contient des informations sur le rôle WVD impliqué dans l’activité, les messages d’erreur qui s’affichent pendant la session, ainsi que des informations sur le client et l’utilisateur. Azure log Analytics peut être configuré pour capturer le journal d’activité créé par l’outil de diagnostic. Voici comment procéder :

1. Créez un espace de travail d’analyse des journaux avec le [portail Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Connectez les ordinateurs Windows à Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Obtenir l’ID d’espace de travail et la clé primaire de votre espace de travail. L’Assistant installation a besoin de ces informations pour configurer correctement l’agent et pour s’assurer qu’il peut communiquer avec Azure Monitor.
1. [Transférer les données de diagnostic vers votre espace de travail](https://go.microsoft.com/fwlink/?linkid=2128284). Vous pouvez transférer les données de diagnostic de votre client WVD vers l’analyse du journal pour votre espace de travail.
1. [Identifier et diagnostiquer les problèmes](https://go.microsoft.com/fwlink/?linkid=2128338) internes ou externes par rapport à WVD.

Pour en savoir plus sur la configuration de l’outil de diagnostic de service pour WVD, consultez [la rubrique use log Analytics for the Diagnostics Feature](https://go.microsoft.com/fwlink/?linkid=2128084).
