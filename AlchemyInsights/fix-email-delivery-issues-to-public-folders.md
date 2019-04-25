---
title: Corriger les problèmes de remise des messages électroniques dans les dossiers publics à extension messagerie
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401326"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Corriger les problèmes de remise des messages électroniques dans les dossiers publics à extension messagerie

Si les expéditeurs externes ne peuvent pas envoyer de messages à vos dossiers publics à extension messagerie et que les expéditeurs reçoivent l'erreur suivante: introuvable **(550 5.4.1)**, vérifiez que le domaine de messagerie du dossier public est configuré en tant que domaine de relais interne au lieu d'un domaine faisant autorité:

1. Ouvrez le [Centre d'administration Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Accédez à **** \> **domaines**de flux de messagerie acceptés, sélectionnez le domaine accepté, puis cliquez sur **modifier**.

3. Dans la page des propriétés qui s'ouvre, si le type de domaine est défini sur **authoritative**, modifiez la valeur sur **relais interne** , puis cliquez sur **Enregistrer**.

Si les expéditeurs externes reçoivent l'erreur « **vous n'avez pas l'autorisation (550 5.7.13)**, exécutez la commande suivante dans [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pour voir les autorisations pour les utilisateurs anonymes dans le dossier public:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Par exemple, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Pour autoriser les utilisateurs externes à envoyer des messages électroniques à ce dossier public, ajoutez le droit d'accès CreateItems à l'utilisateur anonyme. Par exemple, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
