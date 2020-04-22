---
title: Code d’erreur 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703136"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Erreur lors de l’activation d’Office 2013 sur les services Bureau à distance

Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.
  
|**Clé de Registre**|**Type**|**Valeur**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |0,1  <br/> |

Pour plus d’informations, consultez la rubrique [activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL est activée par défaut dans les applications Microsoft 365 pour entreprise et Office 2016. Services Bureau à distance (RDS) était précédemment nommé services Terminal Server.
  