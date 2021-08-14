---
title: Résoudre les problèmes d’installation de DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945929"
---
# <a name="fix-dkim-setup-issues"></a>Résoudre les problèmes d’installation de DKIM

Si vous avez des problèmes d’activation de DKIM pour votre domaine personnalisé, utilisez les étapes suivantes :

- La plupart des problèmes d’installation de DKIM sont liés à des enregistrements DNS incorrects. Vérifiez que l’enregistrement CNAME DKIM **(et non** un enregistrement TXT) est correctement formaté. Pour plus d’informations, consultez cette [rubrique.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Après avoir créé ou mis à jour vos enregistrements DNS DKIM auprès du service d’hébergement DNS de votre domaine (généralement, votre bureau d’enregistrement de domaines), attendez que les enregistrements DNS se propagent.

- Si vous ne pouvez pas créer les enregistrements DKIM DNS dans le Centre d’administration, vous pouvez remplacer par votre domaine personnalisé (par exemple, contoso.com) et exécuter cette commande dans \<CustomDomain\> [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
