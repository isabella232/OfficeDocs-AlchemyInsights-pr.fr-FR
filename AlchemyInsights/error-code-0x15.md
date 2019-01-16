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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288271"
---
Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements Remote Desktop Services (RDS), envisagez d’activer ADAL en modifiant le Registre. 
  
|**Clé de Registre**|**Type**|**Valeur**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Pour plus d’informations, voir [Activer l’authentification moderne pour Office 2013 sur les périphériques Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL est activée par défaut dans Office 365 ProPlus et Office 2016. > Du Bureau à distance (RDS) a été précédemment appelé Services Terminal Server. 
  

