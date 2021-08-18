---
title: Messages électroniques manquants en quarantaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329660"
---
# <a name="missing-emails-in-quarantine"></a>Messages électroniques manquants en quarantaine

Les administrateurs [peuvent afficher, libérer ou supprimer ces messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

In the Microsoft 365 Defender portal at <https://security.microsoft.com> , go to **Review** \> **Quarantine**. Ou, pour aller directement à la page de mise **en** quarantaine, utilisez <https://security.microsoft.com/quarantine> .  

Pour plus d’informations sur les valeurs de recherche/filtre que vous pouvez utiliser, voir Gérer les messages et fichiers mis en quarantaine en tant qu’administrateur [dans EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Les cmdlets que vous utilisez pour afficher et gérer les messages et les fichiers en quarantaine sont :

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): notez que cette cmdlet est uniquement pour les messages, et non pour les fichiers de Coffre Attachments for SharePoint, OneDrive ou Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
