---
title: Corriger les problèmes d’installation de DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765043"
---
# <a name="fix-dkim-setup-issues"></a>Corriger les problèmes d’installation de DKIM

Si vous rencontrez des problèmes d’activation de DKIM pour votre domaine personnalisé, procédez comme suit:

- La plupart des problèmes d’installation de DKIM sont liés à des enregistrements DNS incorrects. Vérifiez que l’enregistrement CNAMe DKIM (et**non** un enregistrement txt) est correctement mis en forme. Pour plus d’informations, consultez cette [rubrique](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Une fois que vous avez créé ou mis à jour vos enregistrements DNS DKIM au niveau du service d’hébergement DNS pour votre domaine (en général, votre bureau d’enregistrement de domaines), attendez que les enregistrements DNS se propagent.

- Si vous ne pouvez pas créer les enregistrements DNS DKIM dans le centre d’administration, \<vous\> pouvez remplacer CustomDomain par votre domaine personnalisé (par exemple, contoso.com) et exécuter cette commande dans [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
