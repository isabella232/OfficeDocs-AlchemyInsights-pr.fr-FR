---
title: Identifier les problèmes liés à Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590276"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifier les problèmes liés à Windows Virtual Desktop

Windows Virtual Desktop Diagnostics n'utilise qu'une seule cmdlet PowerShell, mais contient de nombreux paramètres facultatifs qui permettent de circonscrire et d'isoler les problèmes. Pour commencer : 

1. Téléchargez et importez le module PowerShell Windows Virtual Desktop. Pour plus de détails, voir [Windows Virtual Desktop Cmdlets pour Windows PowerShell .](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Exécutez le cmdlet suivant pour vous connecter à votre compte :
    
    Exemple : `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**REMARQUE :** Toutes les requêtes utilisant PowerShell doivent inclure les paramètres -UserName ou -ActivityID. Pour les capacités de surveillance, voir Utiliser [l'analyse des journaux pour la fonction de diagnostic](https://go.microsoft.com/fwlink/?linkid=2126847) .

Pour filtrer les activités de diagnostic par utilisateur, exécutez la cmdlet suivante :

Exemple : `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Il existe une liste de filtres que vous pouvez exécuter pour diagnostiquer les problèmes. Pour en savoir plus sur le diagnostic des problèmes, reportez-vous à la section [Identifier et diagnostiquer les problèmes de Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Pour en savoir plus sur les erreurs courantes, consultez la rubrique [Scénarios d'erreurs courantes](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
