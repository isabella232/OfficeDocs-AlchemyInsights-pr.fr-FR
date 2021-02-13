---
title: Problème lié aux groupes de sécurité
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162924"
---
# <a name="issue-with-security-groups"></a>Problème lié aux groupes de sécurité

**Si vous obtenez l’erreur réseau AADDS104**

Les règles de groupe de sécurité réseau non valides constituent la cause la plus fréquente d’erreurs réseau pour Azure Active Directory Domain Services (AD DS). Le groupe de sécurité réseau du réseau virtuel doit autoriser l’accès à des ports et à des protocoles spécifiques. Si le groupe de sécurité bloque l’accès à ces ports, la plateforme Azure ne peut pas surveiller, ni mettre à jour le domaine géré. Cela a également un impact sur la synchronisation entre Azure AD et Azure AD DS. Veillez à laisser les ports par défaut ouverts pour éviter une interruption du service.

Si vous souhaitez en savoir plus sur les alertes courantes correspondant aux problèmes de configuration des groupes de sécurité réseau, veuillez consulter la rubrique [Ajouter et vérifier des groupes de sécurité](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
