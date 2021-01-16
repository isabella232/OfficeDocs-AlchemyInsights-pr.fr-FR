---
title: Configurer LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876548"
---
# <a name="configure-ldap"></a>Configurer LDAP

Pour configurer LDAP, faites les choses suivantes :

1. Vérifiez l’état d’état de votre domaine sur [le portail Azure.](https://aka.ms/aadds-health)
1. Assurez-vous qu’un abonnement Azure AD valide est disponible et que les services de domaine Azure AD ont été activés.
1. Le certificat requis pour activer le LDAP sécurisé doit être obtenu auprès d’une autorité de certification publique de confiance ou être un certificat auto-signé.
1. Assurez-vous que le certificat suit les [instructions requises.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificat non valide**
1. Pour renouveler un certificat, suivez les étapes pour créer un certificat et recharger : [Configurez LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Pour résoudre le problème connu avec les alertes LDAP sécurisées dans Les services de domaine Azure Active Directory, consultez [Résoudre les alertes LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
