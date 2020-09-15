---
title: À propos de l’identité dans Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664168"
---
# <a name="about-identity-in-yammer"></a>À propos de l’identité dans Yammer

Nous vous recommandons de suivre les étapes suivantes pour tous les réseaux dans le but d’éviter les problèmes liés à l’identité :

1. Appliquez l’identité Office 365 après la mise en service des comptes Microsoft 365 pour les utilisateurs dans Azure Active Directory pour vérifier que tous les utilisateurs se connectent à l’aide de leur compte Microsoft 365 principal. Pour obtenir davantage d’informations, voir [Appliquer l’identité Office 365 pour les utilisateurs Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Consolidez plusieurs réseaux Yammer. Les configurations Yammer héritées autorisent la connexion de plusieurs réseaux Yammer à un client. Pour obtenir davantage d'informations, consultez l'article [Migration réseau : consolider plusieurs réseaux Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Vous pouvez également appliquer les licences pour Yammer afin de bloquer les utilisateurs de Yammer qui ne disposent pas de licence. Si vous souhaitez en savoir plus, consultez [Gérer les licences utilisateur de Yammer dans Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Enfin, auditez la liste des utilisateurs pour les anciens réseaux Yammer et suspendez les utilisateurs hérités. Il est recommandé de suspendre (désactiver) les utilisateurs au lieu de les supprimer, car leur suppression est irréversible. Pour obtenir davantage d’informations, voir [Audit des utilisateurs de Yammer dans des réseaux connectés à Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) et [Supprimer des utilisateurs](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

En configurant Yammer à l’aide de ces étapes, vous serez également prêt à configurer votre réseau Yammer en mode natif pour Microsoft 365. Pour obtenir davantage d’informations, consultez [Configurer votre réseau Yammer en mode natif pour Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).