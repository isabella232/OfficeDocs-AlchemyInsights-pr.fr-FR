---
title: Code d’erreur 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements Remote Desktop Services (RDS), envisagez d’activer ADAL en modifiant le Registre.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499380"
---
Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements Remote Desktop Services (RDS), envisagez d’activer ADAL en modifiant le Registre. 
  
|**Clé de Registre**|**Type**|**Valeur**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |^1  <br/> |
   
Pour plus d’informations, voir [Activer l’authentification moderne pour Office 2013 sur les périphériques Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL est activée par défaut dans Office 365 ProPlus et Office 2016. > remote Desktop Services (RDS) a été précédemment appelé Services Terminal Server. 
  

