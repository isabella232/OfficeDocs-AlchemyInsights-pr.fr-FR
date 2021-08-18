---
title: Tester la configuration IRM pour les nouvelles fonctionnalités OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899694"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Tester la configuration IRM pour les nouvelles fonctionnalités OME

Pour vérifier que votre locataire Microsoft 365 est configuré pour utiliser les nouvelles fonctionnalités OME, exécutez les applets de commande suivantes quand vous êtes connecté à [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) :


1. Vérifiez la configuration IRM de votre locataire en exécutant `Get-IRMConfiguration`. Assurez-vous que ces valeurs sont définies sur **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. À l’aide de votre domaine, adresse de l’expéditeur et destinataire, exécutez `Test-IRMConfiguration`. Si le test ne réussit pas, examinez votre configuration IRM.

Pour plus d’informations sur la vérification de la configuration IRM, consultez [Vérifier la nouvelle configuration OME dans Exchange Online PowerShell](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).