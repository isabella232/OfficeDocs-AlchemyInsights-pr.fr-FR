---
title: Résoudre les problèmes de remise des e-mails aux dossiers publics à messagerie
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068810"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Résoudre les problèmes de remise des e-mails aux dossiers publics à messagerie

Si les expéditeurs externes ne peuvent pas envoyer de messages vers vos dossiers publics à messagerie et que les expéditeurs reçoivent l’erreur : in trouvé **(550 5.4.1),** vérifiez que le domaine de messagerie du dossier public est configuré en tant que domaine de relais interne au lieu d’un domaine faisant autorité :

1. Ouvrez [le Centre Exchange’administration centrale (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Go to **Mail flow** \> **Accepted domains,** select the accepted domain, and then click **Edit**.

3. Dans la page de propriétés qui s’ouvre, si le type de domaine est définie sur **Faisant** autorité, modifiez la valeur en **relais interne,** puis cliquez sur **Enregistrer**.

Si les expéditeurs externes reçoivent l’erreur que vous **n’avez pas d’autorisation (550 5.7.13),** exécutez la commande suivante dans [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pour voir les autorisations pour les utilisateurs anonymes dans le dossier public :

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Par exemple, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Pour autoriser les utilisateurs externes à envoyer des courriers électroniques à ce dossier public, ajoutez le droit d’accès CreateItems à l’utilisateur Anonyme. Par exemple, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
