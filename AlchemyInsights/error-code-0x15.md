---
title: Code d'0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en éditant le Registre.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316684"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erreur lors de l’activation Office 2013 sur les services Bureau à distance

Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en éditant le Registre.
  
|**Clé de Registre**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

Pour plus d’informations, [voir Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
**Remarque**: ADAL est activée par défaut dans Applications Microsoft 365 pour les grandes entreprises et Office 2016. Les services Bureau à distance (RDS) étaient auparavant nommés Services Terminal Services.
  