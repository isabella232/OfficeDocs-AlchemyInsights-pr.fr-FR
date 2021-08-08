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
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908970"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Tester la configuration IRM pour les nouvelles fonctionnalités OME

Pour vérifier que votre locataire Microsoft 365 est configuré pour utiliser les nouvelles fonctionnalités OME, exécutez les applets de commande suivantes quand vous êtes connecté à [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell) :


1. Vérifiez la configuration IRM de votre locataire en exécutant `Get-IRMConfiguration`. Assurez-vous que ces valeurs sont définies sur **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. À l’aide de votre domaine, adresse de l’expéditeur et destinataire, exécutez `Test-IRMConfiguration`. Si le test ne réussit pas, examinez votre configuration IRM.

Pour plus d’informations sur la vérification de la configuration IRM, consultez [Vérifier la nouvelle configuration OME dans Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).