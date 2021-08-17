---
title: Résolution des erreurs de la mise en suspens de la découverte électronique.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 2a7372c7b20b87c8c774eae4ca4540a3bd19709596405da041eeaa24db310fa7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105386"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Résolution des erreurs de la mise en suspens de la découverte électronique.

Vous rencontrez des problèmes avec les suspensions d'eDiscovery ? Voici quelques bonnes pratiques à prendre en considération :

- Vérifiez l'état de la distribution des mises en suspens.  Si l’état est **Activé (en attente)** ou **Désactivé (en attente)**, attendez que la distribution de suspension soit terminée.
- Fusionnez les mises à jour des suspensions eDiscovery en une seule demande groupée au lieu de mettre à jour la stratégie à plusieurs reprises pour chaque transaction.
- Exécutez la <policyname> Set-CasePolicy -RetryDistribution dans le Centre de sécurité et conformité PowerShell. Pour plus d’informations, consultez [Se connecter à l’interface PowerShell du Centre de sécurité et conformité](/powershell/exchange/connect-to-scc-powershell).

Pour consulter ces paramètres et d’autres meilleures pratiques pour l’atténuation et la résolution des problèmes de mise en suspens de la découverte électronique, consultez [Résoudre les erreurs de mise en suspens de la découverte électronique](/microsoft-365/compliance/hold-distribution-errors).
Pour plus d’informations sur la résolution d’autres problèmes courants de découverte électronique, consultez [Rechercher, résoudre les problèmes et résoudre de découverte électronique courants](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
